---
title: Depanarea problemelor de sign-on unic fără sincope (SSO) bazate pe OIDC
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105790"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Depanarea problemelor de sign-on unic fără sincope (SSO) bazate pe OIDC

- Pentru a afla cum să adăugați o aplicație bazată pe OIDC la entitatea dvs. găzduită Azure, consultați Pornire rapidă: Configurați [sign-on unic (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)bazat pe OIDC pentru o aplicație din entitatea dvs. găzduită Azure Active Directory (Azure AD).
- Pentru mai multe detalii despre aplicațiile care utilizează openID Conectare standard pentru a implementa sign-on unic, consultați Înțelegeți sign-onul unic bazat pe [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Pentru informații în cazul în care alegeți să scrieți codul prin trimiterea și gestionarea directă a solicitărilor HTTP sau utilizând o bibliotecă open-source terță, în loc să utilizați una dintre bibliotecile noastre open-source, consultați Protocoalele noastre de Conectare [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)și OpenID din Serviciu de identitate Microsoft .

**Protocoale**

1. [Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) implicită de acordare - caracteristica definită a grantului implicit este faptul că simbolurile (tokenurile ID sau tokenurile de acces) sunt returnate direct din punctul final /authorize în locul punctului final /token. Acest lucru este utilizat adesea ca parte a fluxului de cod de autorizare, în ceea ce se numește **"flux hibrid" - preluarea simbolului ID** în solicitarea /authorize împreună cu un cod de autorizare. Acest articol descrie cum să programați direct cu protocolul din aplicația dvs. pentru a solicita simboluri de la Azure AD.
2. Serviciu de identitate Microsoft și fluxul de cod de autorizare [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Grantul de cod de autorizare OAuth 2.0 poate fi utilizat în aplicațiile instalate pe un dispozitiv pentru a obține acces la resurse protejate, cum ar fi API-uri web. Utilizând implementarea Serviciu de identitate Microsoft OAuth 2.0, puteți adăuga conectare și acces API la **aplicațiile mobile și desktop.** Acest articol vă arată cum să faceți un program direct față de protocolul din aplicație utilizând orice limbă.
3. Serviciu de identitate Microsoft protocol [Conectare OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) și OpenID : atunci când utilizați implementarea openid Conectare în Serviciu de identitate Microsoft, puteți să adăugați conectare și acces API la aplicațiile dvs. Acest articol vă arată cum să faceți acest lucru independent de limbă și descrie cum să trimiteți și să primiți mesaje HTTP fără a utiliza biblioteci **Microsoft open-source.**
4. Serviciu de identitate Microsoft și fluxul de acreditări [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Puteți utiliza acreditările de client OAuth 2.0 specificate în RFC 6749, numite uneori **OAuth** cu două picioare, pentru a accesa resursele găzduite pe web utilizând identitatea unei aplicații. Acest tip de grant este utilizat de obicei pentru interacțiunile server-la-server care trebuie să ruleze în fundal, fără interacțiune imediată cu un utilizator. Aceste tipuri de aplicații sunt denumite adesea **daemoni sau** **conturi de serviciu.** Acest articol vă arată cum să programați direct față de protocolul din aplicația dvs.
