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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405515"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="63e14-102">Obțineți o listă de aplicații Enterprise</span><span class="sxs-lookup"><span data-stu-id="63e14-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="63e14-103">Pentru a obține o listă **de** aplicații de întreprindere (toate aplicațiile sau filtrate după Nume afișat, ID, URI-uri de identificator etc.) prin comanda Powershell, consultați [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="63e14-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="63e14-104">Pentru a obține o listă de obiecte principale de serviciu (toate obiectele sau filtrate după ID) prin intermediul comenzii Powershell, consultați [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="63e14-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="63e14-105">Dacă doriți să **obțineți o listă de aplicații configurate SAML, următoarele scripturi PowerShell vă** pot ajuta:</span><span class="sxs-lookup"><span data-stu-id="63e14-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="63e14-106">Fiecare aplicație poate fi o aplicație OAuth sau o aplicație SAML (atât aplicații de galerie, cât și aplicații care nu sunt galerie) vor avea două obiecte create în AAD atunci când are loc înregistrarea lor.</span><span class="sxs-lookup"><span data-stu-id="63e14-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="63e14-107">Una se numește Obiect aplicație, iar cealaltă este obiectul Principal serviciu.</span><span class="sxs-lookup"><span data-stu-id="63e14-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="63e14-108">Atunci când dez dispuneți de proprietățile unui obiect principal de serviciu utilizând PowerShell, descoperiți că fiecare aplicație are un anumit număr de Etichete asociate cu ea, cum ar fi:</span><span class="sxs-lookup"><span data-stu-id="63e14-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="63e14-109">Aplicațiile OAuth ar avea o etichetă numită "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="63e14-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="63e14-110">Galeria Aplicațiile SAML ar avea o etichetă numită "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="63e14-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="63e14-111">Aplicațiile NON-Gallery SAML ar avea o etichetă numită "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="63e14-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="63e14-112">Așadar, puteți să utilizați aceste etichete și să a afla ce tip de aplicație este.</span><span class="sxs-lookup"><span data-stu-id="63e14-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="63e14-113">Eticheta "**WindowsAzureActiveDirectoryIntegratedApp" este** comună pentru toate tipurile de aplicații.</span><span class="sxs-lookup"><span data-stu-id="63e14-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="63e14-114">Puteți utiliza următorul fragment pentru a lista toate aplicațiile SAML (atât din galerie, cât și din afara galeriei):</span><span class="sxs-lookup"><span data-stu-id="63e14-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="63e14-115">Pentru mai multe informații, [consultați Identificarea aplicațiilor cu SAML activat în Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="63e14-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="63e14-116">**Găsiți și listați doar aplicațiile web:** utilizați comanda de mai jos pentru a obține toate aplicațiile Azure AD cu tipul de aplicație "Aplicație web/API"</span><span class="sxs-lookup"><span data-stu-id="63e14-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="63e14-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="63e14-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="63e14-118">**Găsiți și listați doar aplicațiile native:** Rulați următoarea comandă pentru a obține toate aplicațiile client nativ (desktop/dispozitiv mobil).</span><span class="sxs-lookup"><span data-stu-id="63e14-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="63e14-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="63e14-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="63e14-120">**Exportați toate detaliile înregistrate ale** aplicației Azure AD în CSV: Comanda de mai jos exportă toate aplicațiile Azure AD cu detalii necesare într-un fișier csv:</span><span class="sxs-lookup"><span data-stu-id="63e14-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="63e14-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="63e14-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="63e14-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Codificare UTF8</span><span class="sxs-lookup"><span data-stu-id="63e14-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="63e14-123">**Trebuie să exportați o listă de aplicații Azure neutilizate** - raport de audit</span><span class="sxs-lookup"><span data-stu-id="63e14-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="63e14-124">Azure AD poate afișa jurnalele de aplicații doar până la 30 de zile, dacă aveți licența Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="63e14-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="63e14-125">Aveți două opțiuni pentru a păstra datele mai mult de 30 de zile.</span><span class="sxs-lookup"><span data-stu-id="63e14-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="63e14-126">Puteți utiliza [API-urile Azure AD Reporting pentru](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) a regăsi datele prin program și a le stoca într-o bază de date.</span><span class="sxs-lookup"><span data-stu-id="63e14-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="63e14-127">Alternativ, puteți integra jurnalele de auditare într-un sistem SIEM terț.</span><span class="sxs-lookup"><span data-stu-id="63e14-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="63e14-128">De asemenea, puteți descărca lista de aplicații pentru toate aplicațiile și aplicațiile proprii de sub Azure Active Directory>Înregistrări aplicații>Descărcați>Toate aplicațiile/Aplicațiile proprii.</span><span class="sxs-lookup"><span data-stu-id="63e14-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="63e14-129">Pentru a obține o listă de aplicații prin MS Graph, consultați Aplicații listă [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) și tipul de resurse aplicație [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="63e14-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
