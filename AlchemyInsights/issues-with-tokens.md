---
title: Probleme cu jetoanele
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917036"
---
# <a name="issues-with-tokens"></a>Probleme cu jetoanele

Pentru a gestiona problemele legate de tokenuri, puteți efectua următorii pași:

1. Puteți specifica durata de viață a unui token Access, ID sau SAML emis de platforma de identitate Microsoft. Puteți să setați vieți token pentru toate aplicațiile din organizație, pentru o aplicație cu mai multe entități găzduite (multi-organizație) sau pentru un anumit director de serviciu din organizația dvs. Pentru mai multe informații, consultați [durata de viață a tokenurilor configurabile în platforma Microsoft Identity (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Jetoanele Access permit clienților să apeleze în siguranță API-uri web protejate și sunt utilizate de API-uri web pentru a efectua autentificarea și autorizarea. Conform specificațiilor OAuth, simbolurile Access sunt șiruri opace fără un format set-unii furnizori de identitate (PSI) utilizează GUID-urile, altele utilizează blobs criptate. Platforma de identitate Microsoft utilizează o varietate de formate de simboluri Access, în funcție de configurația API care acceptă simbolul. Pentru a afla cum poate valida API-ul și a utiliza creanțele dintr-un simbol Access, consultați [simboluri de acces ale platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Biblioteca de autentificare Microsoft (MSAL) acceptă mai multe fluxuri de autentificare pentru utilizare în scenarii de aplicație diferite. Pentru mai multe informații, consultați [fluxurile de autentificare](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Grantul codului de autorizare OAuth 2,0 poate fi utilizat în aplicațiile care sunt instalate pe un dispozitiv pentru a avea acces la resurse protejate, cum ar fi API-uri web. Utilizând implementarea platformei Microsoft Identity din OAuth 2,0, puteți să adăugați conectarea și accesul API la aplicațiile mobile și desktop. Consultați [fluxul de cod de autorizare Microsoft Identity și OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) pentru a programa direct împotriva protocolului din aplicație, utilizând orice limbă.
5. OpenID Connect (OIDC) este un protocol de autentificare bazat pe OAuth 2,0 pe care îl puteți utiliza pentru a vă conecta în siguranță la o aplicație. Atunci când utilizați implementarea Endpoint a platformei Microsoft Identity pentru OpenID Connect, puteți să adăugați conectarea și accesul API la aplicații. [Platforma de identitate Microsoft și protocolul OpenID Connect vă](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) arată cum să faceți acest lucru independent de limbă și cum să trimiteți și să PRIMIȚI mesaje http fără a utiliza nicio bibliotecă Microsoft Open-Source.
    - Punctul final UserInfo face parte din standardul OIDC, proiectat pentru a returna revendicări despre utilizatorul care s-a autentificat. Pentru mai multe informații, consultați [punctul final al platformei de identitate Microsoft UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Apelarea unui API Web într-o aplicație Web utilizând AZURE AD și OpenID Connect sample vă](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) arată cum să creați o aplicație Web MVC care utilizează Azure AD pentru conectare utilizând protocolul OpenID Connect, apoi să apelați un API web sub identitatea utilizatorului conectat, utilizând tokenuri obținute prin OAuth 2,0. Acest eșantion utilizează OpenID Connect ASP .net OWIN middleware și Monica .net.
6. [Configurarea unei aplicații pentru a expune un API web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -în această pornire rapidă, înregistrați un API web cu platforma de identitate Microsoft și expuneți-l în aplicațiile client, adăugând un domeniu de exemplu. Prin înregistrarea API-ului web și expunerea acestuia prin domenii, puteți să furnizați acces bazat pe permisiuni la resursele sale pentru utilizatori autorizați și aplicații client care vă pot accesa API-ul.
7. În Azure Active Directory B2C (Azure AD B2C), fluxul de acreditări ale parolei proprietarului de resurse (ROPC) este un flux de autentificare standard OAuth. În acest flux, o aplicație, denumită și parte care se bazează, schimbă acreditările valide pentru tokenuri. Acreditările includ un ID de utilizator și o parolă. Simbolurile returnate sunt un simbol ID, un token de acces și un token de reîmprospătare. Pentru mai multe informații, consultați [Configurarea unui flux de acreditări de parolă proprietar de resurse în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

