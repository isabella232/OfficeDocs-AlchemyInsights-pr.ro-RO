---
title: Probleme de conectare pentru utilizatorul SSO fără sudură
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935179"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Probleme de conectare pentru utilizatorul SSO fără sudură

După autentificarea utilizatorului, browserul va memora acreditările utilizatorului, astfel încât, în același browser, aplicația să se conecteze automat la același cont. Acest lucru poate îngreuna faptul ca un alt utilizator sau un singur utilizator să se conecteze la mai multe conturi pe un singur dispozitiv. Pentru a rezolva această problemă: 1. Încercați să vă conectați la alt browser. 2. Debifați memoria cache a browserului și/sau modulele cookie și încercați din nou să vă conectați.

Dacă încă întâmpinați probleme de conectare, vă recomandăm următoarele pentru a diagnostica și a automatiza pașii de rezolvare:

1. Instalați [extinderea aplicațiilor mele sigure pentru browser](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) pentru a ajuta Azure Active Directory (Azure AD) să ofere un diagnostic și rezoluții mai bune atunci când utilizați experiența de testare din portalul Azure.
2. Reproducerea erorii utilizând experiența de testare din pagina de configurare a aplicației din portalul Azure. Pentru a afla mai multe, consultați [Depanarea aplicațiilor de sign-on unice bazate pe SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Dacă utilizați experiența de testare din portalul Azure cu extensia de browser securizată a aplicațiilor mele, puteți **ignora pasul 4**.
4. Pentru a deschide pagina de configurare pentru sign-on unic bazat pe SAML:
    - Deschideți [portalul Azure](https://portal.azure.com/) și conectați-vă ca **administrator global** sau **coadministrator**.
    - Deschideți **extensia Azure Active Directory** selectând **toate serviciile** în partea de sus a meniului de navigare principal din partea stângă.
    - Tastați "Azure Active Directory" în caseta de căutare filtrare și selectați elementul **Azure Active Directory** .
    - Selectați **aplicații de întreprindere** din meniul de navigare din stânga-dreapta Azure Active Directory.
    - Selectați **toate aplicațiile** pentru a vizualiza o listă cu toate aplicațiile dvs. Dacă nu vedeți aplicația pe care doriți să o Afișați aici, utilizați controlul de **Filtrare** din partea de sus a **listei toate aplicațiile** și setați opțiunea **Afișare** pentru **toate aplicațiile**.
    - Selectați aplicația pe care doriți să o configurați pentru sign-on unic.
    - După ce se încarcă aplicația, selectați **Sign-on unic** din meniul de navigare din partea stângă a aplicației.
    - Selectați **SSO bazat pe SAML**.
5. Pe baza erorii, pentru a afla mai multe despre pașii recomandați de urmărit, consultați [probleme la conectarea la aplicații configurate pentru sign-on unic bazat pe SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Pentru a depana alte probleme de sign-in de utilizator, consultați următoarele instrucțiuni:
    - [Protocolul single Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Instrucțiuni: Depanarea erorilor de conectare utilizând rapoartele Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Solicitare de consimțământ neașteptată](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Eroare de consimțământ pentru utilizator](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Probleme la conectare din aplicațiile mele](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Eroare la pagina de conectare la aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problemă la conectarea la o aplicație Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
