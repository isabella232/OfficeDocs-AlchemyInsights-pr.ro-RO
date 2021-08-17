---
title: Probleme de conexiune SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084358"
---
# <a name="sso-connection-issues"></a>Probleme de conexiune SSO

1. Urmați [Pornire rapidă: Configurarea proprietăților pentru un ghid de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pentru a configura aplicația.
2. În funcție de aplicație și de opțiunea [de sign-on unic pe care](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) le-ați ales, urmați instrucțiunile corespunzătoare de mai jos:
    - Pentru a **configura** o aplicație unică pentru **sign-on** unic bazat pe SAML, consultați [SAML sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)unic pentru aplicațiile local cu Proxy aplicație.
    - Pentru a configura o **aplicație cloud** **pentru sign-on unic bazat pe parolă,** consultați [Configurarea semnului unic al parolei.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Pentru a configura **o aplicație local** pentru **sign-on** unic prin proxy de aplicație, consultați Seiful de parole pentru [sign-on unic cu Proxy aplicație.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Depanarea problemelor cu proxy-ul** de aplicație: vă recomandăm să începeți cu revizuirea fluxului de depanare, [depanarea](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemelor cu conectorul proxy de aplicație, pentru a determina dacă conectorii proxy de aplicație sunt configurați corect. Dacă încă aveți probleme la conectarea la aplicație, urmați fluxul de depanare din [Depanarea problemelor din aplicația proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Puteți identifica [problemele CORS utilizând](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) instrumentele de depanare a browserului:
    - Lansați browserul și navigați la aplicația web.
    - Apăsați **F12** pentru a duce consola de depanare.
    - Încercați să reproduceți tranzacția și revizuiți mesajul de consolă. O încălcare CORS produce o eroare de consolă cu privire la origine.
    - Unele probleme cu CORS nu pot fi rezolvate, cum ar fi atunci când aplicația dvs. redirecționează către login.microsoft.com pentru autentificare, iar simbolul de acces expiră. Apelul CORS nu reușește. O soluție pentru acest scenariu este extinderea duratei de viață a tokenului de acces, pentru a împiedica expirarea lui în timpul sesiunii utilizatorului. Pentru mai multe informații despre cum să faceți acest lucru, consultați [Configurabile durata de viață a simbolurilor Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Depanarea conectării unice bazate pe **SAML:** vă recomandăm să verificați Problemele cu conectarea la aplicațiile configurate prin sign-on unic bazate pe [SAML,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)pentru a găsi soluții la problemele pe care cel mai probabil le puteți întâmpina.
5. **Depanarea sign-onului** unic bazat pe parolă: vă recomandăm să bifați Depanarea [sign-onului](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)unic bazat pe parolă în Azure AD pentru a găsi soluțiile la problemele pe care cel mai probabil le puteți întâmpina.
6. Pentru probleme de conexiune în timp ce utilizați o rețea VPN, consultați Cum se utilizează sign on unic [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)prin VPN și Wi-Fi vpn.
