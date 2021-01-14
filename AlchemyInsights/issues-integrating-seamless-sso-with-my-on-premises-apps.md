---
title: Probleme cu integrarea SSO fără sudură cu aplicațiile mele locale
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868721"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Probleme cu integrarea SSO fără sudură cu aplicațiile mele locale

Pentru a depana problemele cu integrarea SSO fără sudură cu aplicațiile locale, procedați astfel:

**Pașii recomandați**

1. Pentru a configura o **aplicație locală** pentru **Sign-on unic prin proxy de aplicație**, consultați [arhivarea parolelor pentru sign-on unic cu proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Depanarea problemelor legate de proxy**-ul aplicației: vă recomandăm să începeți să revizuiți fluxul de depanare, să depanați [problemele legate de conectorul proxy al aplicației](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), pentru a determina dacă conectorii proxy ai aplicației sunt configurați corect. Dacă încă întâmpinați probleme la conectarea la aplicație, urmați pașii de depanare din [problemele de aplicație proxy pentru aplicații de depanare](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Puteți [identifica problemele CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizând următoarele instrumente de depanare a browserului:
    1. Lansați browserul și navigați la aplicația web.
    1. Apăsați **F12** pentru a afișa consola de depanare.
    1. Încercați să reproduceți tranzacția și revizuiți mesajul consolei. O încălcare CORS produce o eroare de consolă despre origine.
    1. Unele probleme CORS nu pot fi rezolvate, cum ar fi atunci când aplicația redirecționează login.microsoftonline.com să se autentifice și simbolul Access expiră. Apelul CORS nu reușește. O soluție pentru acest scenariu este să extindeți durata de viață a tokenului de acces, pentru a împiedica expirarea acestuia în timpul sesiunii unui utilizator. Pentru mai multe informații despre cum să procedați, consultați [durată de viață simbolică configurabilă în platforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documente recomandate**

- [Cum se configurează sign-on unic într-o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML sign-on unic pentru aplicațiile locale cu proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Înțelegerea și rezolvarea problemelor legate de proxy-ul aplicației Azure Active Directory CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Depanarea configurațiilor constrânse de delegare Kerberos pentru proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)