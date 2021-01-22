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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935157"
---
# <a name="sso-connection-issues"></a>Probleme de conexiune SSO

1. Urmăriți [pornire rapidă: Configurați proprietățile pentru un](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ghid de aplicație pentru a configura aplicația.
2. În funcție de aplicația și de [opțiunea de sign-on unic pe](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) care ați ales-o, urmați instrucțiunile corespunzătoare de mai jos:
    - Pentru a configura o **aplicație locală** pentru **Sign-on unic bazat pe SAML**, consultați [SAML single-sign-on pentru aplicațiile locale cu proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Pentru a configura o **aplicație Cloud** pentru **Sign-on unic bazat pe parole**, consultați  [Configurarea conectării unice a parolei](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Pentru a configura o **aplicație locală** pentru **Sign-on unic prin proxy de aplicație**, consultați [arhivarea parolelor pentru sign-on unic cu proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Depanarea problemelor legate de proxy**-ul aplicației: vă recomandăm să începeți să revizuiți fluxul de depanare, să depanați [problemele legate de conectorul proxy al aplicației](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), pentru a determina dacă conectorii proxy ai aplicației sunt configurați corect Dacă încă întâmpinați probleme la conectarea la aplicație, urmați fluxul de depanare din [problemele de aplicație proxy de depanare a aplicațiilor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Puteți [identifica problemele CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizând instrumente de depanare pentru browser:
    - Lansați browserul și navigați la aplicația web.
    - Apăsați **F12** pentru a afișa consola de depanare.
    - Încercați să reproduceți tranzacția și revizuiți mesajul consolei. O încălcare CORS produce o eroare de consolă despre origine.
    - Unele probleme CORS nu pot fi rezolvate, cum ar fi atunci când aplicația redirecționează login.microsoft.com să se autentifice și simbolul Access expiră. Apelul CORS nu reușește. O soluție pentru acest scenariu este să extindeți durata de viață a tokenului de acces, pentru a împiedica expirarea acestuia în timpul sesiunii unui utilizator. Pentru mai multe informații despre cum să procedați, consultați [durată de viață simbolică configurabilă în platforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Depanarea conectării unice bazate pe SAML**: vă recomandăm să verificați dacă aveți [probleme la conectarea la aplicațiile configurate pentru sign-on unic bazat pe SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), pentru a găsi soluțiile la problemele pe care le puteți întâmpina cel mai probabil.
5. **Depanarea conectării unice bazate pe parole**: vă recomandăm să verificați [Depanarea conectării unice bazate pe parolă în Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), pentru a găsi soluțiile la problemele pe care le puteți întâmpina cel mai probabil.
6. Pentru probleme de conexiune în timp ce utilizați o rețea VPN, consultați [cum să utilizați sign on unic (SSO) prin conexiuni VPN și Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
