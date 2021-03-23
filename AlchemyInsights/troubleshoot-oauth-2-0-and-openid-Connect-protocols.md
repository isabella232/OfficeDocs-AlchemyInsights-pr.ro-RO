---
title: Depanarea protocoalelor de conectare OAuth 2,0 și OpenID
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037701"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Depanarea protocoalelor de conectare OAuth 2,0 și OpenID

Pentru a rezolva problemele de conectare OAuth 2,0 și OpenID, efectuați următorii pași recomandate:

Consultați următoarele articole care sunt asociate cu configurarea și depanarea protocoalelor de conectare OAuth 2,0 și OpenID:

- [Microsoft Identity Platform și OAuth 2,0 codul de autorizare](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -acest articol descrie cum să programați direct împotriva **fluxului cod Grant (PKCE)** din aplicație, utilizând orice limbă.
- [Platforma de identitate Microsoft și fluxul de acreditări client 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -acest articol descrie cum să programați direct împotriva **fluxului de acreditări client** în aplicația dvs.
- [Acreditări de parolă pentru proprietarii de resurse Microsoft Identity și OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -acest articol descrie cum să programați direct împotriva **fluxului ROPC** din aplicație.
    - Platforma de identitate Microsoft acceptă doar ROPC pentru entități găzduite Azure AD, nu și pentru conturile personale. Acest lucru înseamnă că trebuie să utilizați un punct final specific entității găzduite **https://login.microsoftonline.com/{TenantId_or_Name}) (** sau punctul final al **organizațiilor** .
    - Conturile personale care sunt invitate la o entitate găzduită Azure AD nu pot utiliza ROPC.
    - Conturile care nu au parole nu se pot conecta prin ROPC. Pentru acest scenariu, vă recomandăm să utilizați în schimb un alt flux pentru aplicație.
    - Dacă utilizatorii trebuie să utilizeze [autentificarea multi-factor (AMF)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) pentru a vă conecta la aplicație, acesta va fi blocat.
    - ROPC nu este acceptat în scenariile de [federație de identitate hibridă](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (de exemplu, Azure AD și ADFS utilizate pentru a autentifica conturile locale). Dacă utilizatorii sunt redirecționați pe pagini complete către un furnizor de identitate local, Azure AD nu poate testa numele de utilizator și parola pentru respectivul furnizor de identitate. [Autentificarea directă](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) este acceptată cu ROPC, totuși.
    - O excepție de la un scenariu de federație de identitate hibridă ar fi următoarele: Politica de descoperire acasă Realm cu **AllowCloudPasswordValidation** setată la **True** va permite ca fluxul ROPC să funcționeze pentru utilizatorii federativi atunci când parola locală este sincronizată cu Cloud. Pentru mai multe informații, consultați [Activarea autentificării directe ROPC a utilizatorilor federativi pentru aplicațiile moștenite](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Platforma de identitate Microsoft și OAuth 2,0 în numele fluxului](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) -acest articol descrie cum să programați direct împotriva **fluxului în numele (OBO)** în aplicația dvs.
- [Platforma de identitate Microsoft și protocolul OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -acest articol vă arată cum să implementați protocolul OpenID Connect independent de limbă și descrie cum să trimiteți și să PRIMIȚI mesaje http fără a utiliza nicio bibliotecă Microsoft Open-Source.

**Simboluri de acces**

[Simboluri de acces ale platformei Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Aflați cum poate valida API-ul și utiliza creanțele dintr-un simbol Access. Toate documentația din acest articol, cu excepția cazului în care se menționează, se aplică doar la tokenurile emise pentru API-uri pe care le-ați înregistrat. Nu se aplică tokenurilor emise pentru API-urile deținute de Microsoft și nici acele simboluri nu pot fi utilizate pentru a valida modul în care platforma de identitate Microsoft va emite tokenuri pentru un API pe care îl creați.

**Configurație aplicație**

[Restricții și limite pentru redirecționare URL-uri (răspuns)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) -Aflați cum să configurați uri redirecționare (URL răspuns). Un URL de redirecționare sau un URL de răspuns este locația în care serverul de autorizare trimite utilizatorul după ce aplicația a fost autorizată cu succes și a acordat un cod de autorizare sau un token de acces. Serverul de autorizare trimite codul sau simbolul la URI redirecționare; prin urmare, este important să înregistrați locația corectă ca parte a procesului de înregistrare a aplicațiilor.

**Asigurarea accesului la aplicații**

[Tutorial: dezvoltarea și planificarea accesului pentru un punct final SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) -acest articol descrie cum să construiți un punct final SCIM și să vă integrați cu serviciul de asigurare a accesului la AAD.


