---
title: Configurarea proxy-ului aplicației
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885525"
---
# <a name="app-proxy-configuration"></a>Configurarea proxy-ului aplicației

1. Pentru a înțelege cum să configurați o aplicație proxy de aplicație din Azure AD pentru a expune aplicațiile locale în cloud, consultați [cum se configurează o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Sign-on unic (SSO) permite utilizatorilor să acceseze o aplicație fără a se autentifica de mai multe ori. Permite autentificarea unică să aibă loc în cloud, împotriva Azure Active Directory și permite serviciului sau conectorului să imite utilizatorul pentru a finaliza toate provocările suplimentare de autentificare din aplicație. Pentru a afla mai multe, consultați [cum se configurează sign-on unic la o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Utilizați [acest articol](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) pentru a depana problemele uzuale cu care se confruntă persoanele atunci când creați o aplicație proxy de aplicație nouă.
4. Dacă întâmpinați o problemă la configurarea autentificării back-end la aplicație, poate fi necesar să [depanați configurațiile de delegare constrânse Kerberos pentru proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) -ul aplicației sau să urmați instrucțiunile pentru [Configurarea aplicației cu PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) pentru a rezolva problema.
