---
title: Depanarea problemelor cu sign-on unic (SSO) bazat pe OIDC
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
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747128"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Depanarea problemelor cu sign-on unic (SSO) bazat pe OIDC

- Pentru a afla cum să adăugați o aplicație bazată pe OIDC la entitatea găzduită Azure, consultați [pornire rapidă: Configurați sign-on unic (SSO) bazat pe OIDC pentru o aplicație din entitatea găzduită Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Pentru mai multe detalii despre aplicațiile care utilizează standardul OpenID Connect pentru a implementa sign-on unic, consultați [înțelegerea conectării unice bazate pe OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Pentru informații în cazul în care alegeți să scrieți codul prin trimiterea și manipularea directă a solicitărilor HTTP sau pentru a utiliza o bibliotecă de surse deschise de la terți, în loc să utilizați una dintre bibliotecile noastre Open-Source, consultați [OAuth 2,0 și OpenID Connect protocoale pe platforma de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protocoalele**

1. [Platforma de identitate Microsoft și fluxul de granturi implicit](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) -caracteristica definitorie a grantului implicit este faptul că tokenurile (token-ul ID sau tokenurile de acces) sunt returnate direct din punctul final/Authorize în locul punctului final/token. Acest lucru este utilizat deseori ca parte a fluxului de cod de autorizare, în ceea ce se numește **"flux hibrid"-recuperarea tokenului ID la solicitarea/Authorize, împreună cu un cod de autorizare**. Acest articol descrie cum să programați direct împotriva protocolului din aplicație pentru a solicita tokenuri de la Azure AD.
2. [Microsoft Identity Platform și OAuth 2,0 codul de autorizare](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -codul de autorizare OAuth 2,0 poate fi utilizat în aplicațiile care sunt instalate pe un dispozitiv pentru a avea acces la resurse protejate, cum ar fi API-uri web. Utilizând implementarea platformei Microsoft Identity din OAuth 2,0, puteți **adăuga conectarea și accesul API la aplicațiile mobile și desktop**. Acest articol descrie cum să programați direct împotriva protocolului din aplicație utilizând orice limbă.
3. [Platforma de identitate Microsoft și protocolul OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -atunci când utilizați implementarea platformei de identitate Microsoft a OpenID Connect, puteți să adăugați conectarea și accesul API la aplicații. Acest articol vă arată cum să faceți acest lucru independent de limbă și descrie cum să **trimiteți și să primiți mesaje http fără a utiliza nicio bibliotecă Microsoft Open-Source**.
4. [Platforma de identitate Microsoft și fluxul de acreditări client 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -puteți utiliza grantul de acreditări client OAuth 2,0 specificat în RFC 6749, denumit uneori **OAuth cu două picioare**, pentru a accesa resursele găzduite de web, utilizând identitatea unei aplicații. Acest tip de Grant este utilizat frecvent pentru interacțiunile server-la-server care trebuie să ruleze în fundal, fără interacțiune imediată cu un utilizator. Aceste tipuri de aplicații sunt denumite adesea **daemoni** sau **conturi de serviciu**. Acest articol descrie cum să programați direct împotriva protocolului în aplicația dvs.
