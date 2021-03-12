---
title: Probleme cu linkuri și cu URL-uri
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707894"
---
# <a name="issues-with-links-and-urls"></a>Probleme cu linkuri și cu URL-uri

URI-uri de redirecționare/URL-uri de răspuns (ambele expresii sunt interschimbabile) sunt URL-urile utilizate de platforma de identitate Microsoft pentru a returna simbolurile solicitate de aplicații. Pentru mai multe informații privind aceste URL-uri, consultați articolele de mai jos:

- [Fluxuri de autentificare și scenarii de aplicație](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Informații despre URI-urile de redirecționare din pagina **Înregistrare aplicații** pentru fiecare scenariu.
- [Restricții și limite pentru URI de redirecționare/URL de răspuns](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nu știu cum să înregistrez URI-ul de redirecționare/URL-ul răspuns corect pentru aplicația mea**

Când vă conectați cu aplicația pe care o dezvoltați, dacă caseta de dialog de conectare afișează **AADSTS50011: URL-ul de răspuns specificat în solicitare nu se potrivește cu URL-urile de răspuns configurate pentru aplicație <your app ID>**, va trebui să adăugați la înregistrarea aplicației dvs., URI-ul de redirecționare utilizat de codul dvs. în solicitarea de simbol către platforma de identitate Microsoft.

Pentru a adăuga un URL de răspuns, accesați fila **Autentificare** din pagina dvs. de **înregistrare a aplicațiilor** din portalul Microsoft Azure și adăugați o intrare în secțiunea **Redirecționare URI-uri.**. Valoarea pe care trebuie să o introduceți depinde de tipul de aplicație pe care o creați, astfel cum este descris mai jos:

- Pentru aplicațiile web și aplicațiile cu o singură pagină, URL-ul de răspuns este un URL din aplicația dvs. Consultați [Înregistrarea aplicațiilor cu o singură pagină](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) sau [Înregistrarea unei aplicații web utilizând portalul Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Pentru aplicațiile desktop, valoarea pe care trebuie să o alegeți depinde de:
    - platformă (MacOS este diferită de Windows sau Linux)
    - modul în care obțineți simbolul (interactiv, cu fluxul de cod de dispozitiv, cu autentificare Windows integrată [IWA] sau cu nume de utilizator/parolă).
    Pentru detalii, consultați [Aplicații desktop - Înregistrare aplicații- URI de redirecționare](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Pentru aplicațiile mobile, URI-ul de redirecționare depinde de:
    - platformă (iOS/Android/UWP)
    - informațiile utilizate pentru a vă crea aplicația, precum ID-ul pachetului din iOS, precum și numele pachetului și hashul de semnătură de pe Android. Înregistrarea aplicației portal Microsoft Azure vă va ajuta. Pentru detalii, consultați [configurarea platformei și redirecționarea URI-urilor](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> API-urile web și unele moduri silențioase de a obține simboluri (IWA și nume de utilizator/parolă) nu necesită un URI de redirecționare.

**Am implementat aplicația mea web și, atunci când testez aplicația implementată, primesc un mesaj de nepotrivire URL de răspuns**

Adăugați URI-uri de redirecționare pentru toate locațiile în care implementați aplicația dvs. web. Pentru mai multe informații, consultați [Înregistrarea unei aplicații web utilizând portalul Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Adăugați URI de redirecționare pentru o locație imediat după ce ați implementat aplicația în acea locație.

**Nu pot înregistra suficiente URL-uri de răspuns**

Aveți un ISV și aveți unul sau mai multe URI-uri de redirecționare pentru fiecare client al dvs. Doriți să migrați de la ADAL/Azure AD v1.0 la MSAL/platforma de identitate Microsoft și ați atinse [numărul maxim de URI-uri de redirecționare](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Pentru a remedia această problemă, [adăugați URI-uri de redirecționare la conturile principale de serviciu](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) care corespund fiecăruia dintre clienții dvs.
