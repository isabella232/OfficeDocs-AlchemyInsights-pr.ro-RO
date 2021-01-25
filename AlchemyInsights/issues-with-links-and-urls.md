---
title: Probleme cu linkurile și adresele URL
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974751"
---
# <a name="issues-with-links-and-urls"></a>Probleme cu linkurile și adresele URL

Redirecționarea URL-urilor/răspunsurilor (ambele expresii sunt interschimbabile) sunt adresele URL utilizate de platforma Microsoft Identity pentru a returna jetoanele solicitate de aplicație. Pentru informații despre aceste adrese URL, consultați următoarele articole:

- [Fluxurile de autentificare și scenariile de aplicație](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -informații despre redirecționarea URIs în pagina de **înregistrare a aplicației** pentru fiecare scenariu.
- [Redirecționarea restricțiilor și limitelor pentru URL-URI de răspuns](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nu știu cum să înregistrez adresa URL redirecționare dreapta/răspuns pentru aplicația mea**

Atunci când vă conectați cu aplicația pe care o dezvoltați, dacă dialogul de conectare afișează **AADSTS50011: adresa URL de răspuns specificată în solicitare nu se potrivește cu URL-urile de răspuns configurate pentru <your app ID> aplicație**, va trebui să adăugați la înregistrarea aplicației dvs., să REdirecționați uri pe care codul le-a utilizat în solicitarea tokenului la platforma de identitate Microsoft.

Pentru a adăuga un URL de răspuns, accesați fila **autentificare** din pagina de **înregistrare a aplicației** din portalul Azure și adăugați o intrare în secțiunea **redirecționare URIs** . Redirecționare URIs sunt tastate (web sau mobil/desktop). Valoarea pe care trebuie să o introduceți depinde de tipul de aplicație pe care o construiți, așa cum se descrie mai jos:

- Pentru aplicațiile cu o singură pagină și pentru aplicațiile web, adresa URL a răspunsului este un URL în aplicația dvs. Vedeți [înregistrarea aplicațiilor pe o singură pagină](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) sau [înregistrați o aplicație de aplicație Web utilizând Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Pentru aplicațiile desktop, valoarea pe care trebuie să o alegeți depinde de:
    - Platforma (MacOS este diferită de Windows sau Linux)
    - modul în care achiziționați simbolul (interactiv, cu fluxul de coduri de dispozitiv, cu autentificarea Windows integrată [IWA] sau cu numele de utilizator/parola).
    Pentru detalii, consultați [aplicații Desktop-înregistrare aplicație-redirecționare uri](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Pentru aplicațiile mobile, e-URI de redirecționare depinde de:
    - Platforma (iOS/Android/UWP)
    - informațiile utilizate pentru a vă construi aplicația, cum ar fi ID-ul pachetului în iOS, precum și numele pachetului și hash-ul de semnătură pe Android, înregistrarea aplicației Azure portal vă va ajuta. Pentru detalii, consultați [Configurarea platformelor și redirecționarea URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> API-uri web și câteva dintre modalitățile de a achiziționa tokenuri (IWA și username/password) nu necesită un URI redirecționare.

**Am implementat aplicația Web și când testez aplicația implementată, primesc un mesaj de nepotrivire URL răspuns**

Adăugați redirecționare URIs pentru toate locațiile în care implementați aplicația web. Pentru mai multe informații, consultați [înregistrarea unei aplicații de aplicație Web utilizând Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Adăugați URI de redirecționare pentru o locație imediat după ce ați implementat aplicația în acea locație.

**Nu pot înregistra suficient URL-uri de răspuns**

Sunteți un ISV și aveți una sau mai multe URIs de redirecționare pentru fiecare client al dumneavoastră. Doriți să migrați de la Monica/Azure AD v 1.0 la MSAL/platforma de identitate Microsoft și ați atins [numărul maxim de redirecționare URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Pentru a rezolva această problemă, [Adăugați redirecționare URIs la directori de servicii](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) care corespund fiecăruia dintre clienții dvs.
