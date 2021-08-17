---
title: Obțineți o listă de aplicații Enterprise
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116740"
---
# <a name="get-a-list-of-enterprise-applications"></a>Obțineți o listă de aplicații Enterprise

1. Pentru a obține o listă **de** aplicații de întreprindere (toate aplicațiile sau filtrate după Nume afișat, ID, URI-uri de identificator etc.) prin comanda Powershell, consultați [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Pentru a obține o listă de obiecte principale de serviciu (toate obiectele sau filtrate după ID) prin intermediul comenzii Powershell, consultați [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Dacă doriți să **obțineți o listă de aplicații configurate SAML, următoarele scripturi PowerShell vă** pot ajuta:

    Fiecare aplicație poate fi o aplicație OAuth sau o aplicație SAML (atât aplicații de galerie, cât și aplicații care nu sunt galerie) vor avea două obiecte create în AAD atunci când are loc înregistrarea lor. Una se numește Obiect aplicație, iar cealaltă este obiectul Principal serviciu. Atunci când dez dispuneți de proprietățile unui obiect principal de serviciu utilizând PowerShell, descoperiți că fiecare aplicație are un anumit număr de Etichete asociate cu ea, cum ar fi:

    - Aplicațiile OAuth ar avea o etichetă numită "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Galeria Aplicațiile SAML ar avea o etichetă numită "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Aplicațiile NON-Gallery SAML ar avea o etichetă numită "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Așadar, puteți să utilizați aceste etichete și să a afla ce tip de aplicație este. Eticheta "**WindowsAzureActiveDirectoryIntegratedApp" este** comună pentru toate tipurile de aplicații. Puteți utiliza următorul fragment pentru a lista toate aplicațiile SAML (atât din galerie, cât și din afara galeriei):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Pentru mai multe informații, [consultați Identificarea aplicațiilor cu SAML activat în Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Găsiți și listați doar aplicațiile web:** utilizați comanda de mai jos pentru a obține toate aplicațiile Azure AD cu tipul de aplicație "Aplicație web/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Găsiți și listați doar aplicațiile native:** Rulați următoarea comandă pentru a obține toate aplicațiile client nativ (desktop/dispozitiv mobil).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exportați toate detaliile înregistrate ale** aplicației Azure AD în CSV: Comanda de mai jos exportă toate aplicațiile Azure AD cu detalii necesare într-un fișier csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Codificare UTF8

7. **Trebuie să exportați o listă de aplicații Azure neutilizate** - raport de audit

    Azure AD poate afișa jurnale de aplicații doar până la 30 de zile, dacă aveți Licență de Premium Azure AD.
    Aveți două opțiuni pentru a păstra datele mai mult de 30 de zile. Puteți utiliza [API-urile Azure AD Reporting pentru](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) a regăsi datele prin program și a le stoca într-o bază de date. Alternativ, puteți integra jurnalele de auditare într-un sistem SIEM terț.

    De asemenea, puteți descărca lista de aplicații pentru toate aplicațiile și aplicațiile proprii de sub Azure Active Directory>Înregistrări aplicații>Descărcați>Toate aplicațiile/Aplicațiile proprii.

    Pentru a obține o listă de aplicații prin intermediul MS Graph, consultați List [applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) și tipul de resursă aplicație [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
