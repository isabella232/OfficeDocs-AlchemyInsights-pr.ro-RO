---
title: Probleme cu integrarea SSO perfect cu aplicațiile mele locale
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028304"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Probleme cu integrarea SSO perfect cu aplicațiile mele locale

Pentru a depana problemele cu integrarea SSO perfectă cu aplicațiile local, acțiunile următoare:

**Pași recomandați**

1. Pentru a configura **o aplicație local** pentru **sign-on** unic prin proxy de aplicație, consultați Seiful de parole pentru [sign-on unic cu Proxy aplicație.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Depanarea problemelor cu proxy-ul** de aplicație: vă recomandăm să începeți cu revizuirea fluxului de depanare, [depanarea](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemelor cu Conector proxy de aplicație, pentru a determina dacă conectorii proxy de aplicație sunt configurați corect. Dacă încă aveți probleme la conectarea la aplicație, urmați pașii de depanare [din Depanarea problemelor de aplicație proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Puteți identifica [problemele CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizând următoarele instrumente de depanare a browserului:
    1. Lansați browserul și navigați la aplicația web.
    1. Apăsați **F12** pentru a duce consola de depanare.
    1. Încercați să reproduceți tranzacția și revizuiți mesajul de consolă. O încălcare CORS produce o eroare de consolă cu privire la origine.
    1. Unele probleme cu CORS nu pot fi rezolvate, cum ar fi atunci când aplicația dvs. redirecționează către site-login.microsoftonline.com pentru autentificare, iar simbolul de acces expiră. Apelul CORS nu reușește. O soluție pentru acest scenariu este extinderea duratei de viață a tokenului de acces, pentru a împiedica expirarea lui în timpul sesiunii utilizatorului. Pentru mai multe informații despre cum să faceți acest lucru, consultați [Configurabile durata de viață a simbolurilor Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documente recomandate**

- [Cum se configurează sign-onul unic într-o aplicație Proxy aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Sign-on unic SAML pentru aplicațiile local cu proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Înțelegeți și rezolvați Azure Active Directory CORS pentru proxy-ul de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Depanarea configurațiilor de delegare constrânse ale lui Kerberos pentru Proxy aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)