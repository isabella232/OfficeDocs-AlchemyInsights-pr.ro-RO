---
title: Configurare sign-on unic perfect (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402279"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurare sign-on unic perfect (SSO)

**Configurarea aplicațiilor**

1. Ar trebui să obțineți valorile de la distribuitorul de aplicații. Puteți să introduceți manual valorile sau să încărcați un fișier de metadate pentru a extrage valoarea câmpurilor.
2. Multe aplicații au fost deja preconfigurate pentru a funcționa cu Azure AD. Aceste aplicații sunt listate în galeria de aplicații pe care le puteți naviga atunci când adăugați o aplicație la entitatea găzduită Azure AD. Seria [de pornire rapidă](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vă ghidează prin proces.
3. Pentru a crea o aplicație care nu este galerie, puteți să faceți clic pe **+ Creați propriul** buton Aplicație și să dați un nume Aplicației.
    - În mod implicit, aceasta **va** selecta Integrați orice altă aplicație pe care nu o găsiți în galerie, care este opțiunea corectă pentru aplicațiile Non-galerie.
    - După ce hit **Create** after putting the name for the application, it will create a new Non-gallery Enterprise Application.
    - Apoi puteți naviga la **Sign-on** unic sub Gestionați aplicația și veți putea vedea diferite tehnici pentru implementarea în mediul dvs. 

**Configurați SSO perfect pentru o anumită aplicație**

Pentru aplicațiile din galerie, veți găsi instrucțiuni detaliate, pas cu pas. Pentru a accesa pașii pe care îi puteți parcurge într-o listă cu toate tutorialele de configurare a aplicațiilor de la Tutorialele de configurare a [aplicațiilor SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurarea SSO bazat pe SAML**

1. [Pornire rapidă: Configurați sign-on unic (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)bazat pe SAML pentru o aplicație din entitatea găzduită Azure Active Directory (Azure AD).
2. Pentru a afla mai multe despre opțiunea bazată pe SAML pentru sign-on unic, consultați [Înțelegeți sign-onul](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)unic bazat pe SAML.
3. Pentru a afla despre solicitările de autentificare SAML 2.0 și răspunsurile pe care Le acceptă Azure Active Directory (Azure AD) pentru single Sign-On (SSO), consultați protocolul [SAML unic Sign-On.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Pentru a afla cum să creați și să configurați o sign-on unic (SSO) bazat pe SAML pentru aplicația dvs. în Azure Active Directory (Azure AD) utilizând API Microsoft Graph, consultați Configurarea [sign-onului](https://docs.microsoft.com/graph/application-saml-sso-configure-api)unic bazat pe SAML pentru aplicația dvs. utilizând API Microsoft Graph.
5. Pentru a afla cum utilizează Azure AD protocolul SAML, consultați Cum utilizează platforma [de identitate Microsoft protocolul SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Configurarea simbolurilor și solicitărilor**

1. [Cum să: particularizați solicitările emise în simbolul SAML pentru aplicațiile de întreprindere.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Pentru a afla cum să configurați solicitări folosind PowerShell, consultați Cum să: Particularizați solicitările omise în simboluri pentru o anumită aplicație într-o [entitate găzduită (Previzualizare)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Pentru a afla cum să configurați solicitările opționale, consultați [Cum să: Oferiți solicitări opționale aplicației dvs.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Pentru a afla cum să utilizați atributele extensiei schemei de director pentru a trimite date de utilizator aplicațiilor în solicitările de simboluri, consultați Utilizarea atributelor extensiei schemei de director [în solicitări.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Pentru a afla cum să configurați durata de viață a simbolurilor, consultați Configurabil durata de viață a [simbolurilor pe platforma de identitate Microsoft (previzualizare).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. Configurarea politicilor pe durata de viață a [simbolurilor (previzualizare)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - În acest articol, vom descrie un scenariu de politică obișnuit care vă poate ajuta să impuneți reguli noi pe durata de viață a simbolurilor. În exemplu, aflați cum să creați o politică ce necesită ca utilizatorii să se autentifice mai frecvent în aplicația web.

**Depanarea configurării SSO**

- Pentru întrebări frecvente despre sign-on unic perfect Azure Active Directory (SSO Sign-On perfectă), consultați [Sign-on unic perfect Azure Active Directory: Întrebări frecvente.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Pentru informații de depanare despre problemele uzuale cu privire la Azure Active Directory (Azure AD) Sign-on unic perfect Sign-On (SSO perfectă), consultați Depanarea [sign-on](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)unic perfect Azure Active Directory.
