---
title: Configurați sign-on unic (SSO) fără sudură
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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841675"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurați sign-on unic (SSO) fără sudură

**Configurarea aplicațiilor**

1. Trebuie să obțineți valorile de la furnizorul aplicației. Puteți să introduceți manual valorile sau să încărcați un fișier de metadate pentru a extrage valoarea câmpurilor.
2. Multe aplicații au fost deja pre-configurate pentru a funcționa cu Azure AD. Aceste aplicații sunt listate în Galeria de aplicații pe care le puteți parcurge atunci când adăugați o aplicație la entitatea găzduită Azure AD. [Seria de pornire rapidă](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vă ajută să parcurgeți procesul.
3. Pentru a crea o aplicație non-Galerie, puteți să faceți clic pe **+ să creați propriul** buton de aplicație și să dați un nume aplicației.
    - În mod implicit, va selecta **integrarea oricărei alte aplicații pe care nu o găsiți în Galerie** , care este opțiunea corectă pentru aplicațiile non-Galerie.
    - După ce ați lovit **Creați** după ce ați introdus numele aplicației, acesta va crea o nouă aplicație de întreprindere non-Galerie.
    - Apoi, puteți naviga la **Sign-on unic** sub **gestionarea** aplicației respective și veți putea vedea tehnici diferite pentru a-l implementa în mediul dvs.

**Configurarea SSO fără sudură pentru o aplicație specifică**

Pentru aplicațiile din Galerie veți găsi instrucțiuni detaliate, pas cu pas. Pentru a accesa pașii pe care îi puteți parcurge o listă cu toate tutorialele de configurare a aplicațiilor la [Tutoriale de configurare a aplicațiilor SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Configurarea SSO bazat pe SAML**

1. [Pornire rapidă: Configurați sign-on unic bazat pe SAML (SSO) pentru o aplicație din entitatea găzduită Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Pentru a afla mai multe despre opțiunea bazat pe SAML pentru sign-on unic, consultați [înțelegerea conectării unice bazate pe SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Pentru a afla despre solicitările de autentificare SAML 2,0 și răspunsurile pe care le acceptă Azure Active Directory (Azure AD) pentru o singură Sign-On (SSO), consultați [protocolul single Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Pentru a afla cum să creați și să configurați un sign-on unic bazat pe SAML (SSO) pentru aplicația din Azure Active Directory (Azure AD) utilizând Microsoft Graph API, consultați [Configurarea conectării unice bazate pe SAML pentru aplicația dvs., utilizând API-ul Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Pentru a afla cum utilizează Azure AD protocolul SAML, consultați [modul în care platforma de identitate Microsoft utilizează protocolul SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Configurarea tokenurilor și a revendicărilor**

1. [Instrucțiuni: particularizați creanțele emise în aplicația token pentru aplicații Enterprise](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Pentru a afla cum să configurați revendicările utilizând PowerShell, consultați instrucțiuni [: Particularizarea creanțelor emise în tokenuri pentru o anumită aplicație într-o entitate găzduită (Previzualizare)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Pentru a afla cum să configurați creanțele opționale, consultați [cum să: furnizați solicitări opționale aplicației dvs](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Pentru a afla cum să utilizați atributele de extensie a schemelor directoare pentru trimiterea de date de utilizator la aplicații în creanțe Token, consultați [Utilizarea atributelor de extensie a schemelor directoare în creanțe](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Pentru a afla cum să configurați duratele de viață ale tokenurilor, consultați [durată de viață simbolică configurabilă în platforma Microsoft Identity (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Configurarea politicilor token Lifetime (Preview)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -în acest articol, parcurgem un scenariu politic comun care vă poate ajuta să Impuneți reguli noi pentru durata de viață a tokenului. În exemplu, veți învăța cum să creați o politică care necesită ca utilizatorii să se autentifice mai frecvent în aplicația web.

**Depanarea configurației SSO**

- Pentru întrebări frecvente despre Azure Active Directory fără sudură single Sign-On (SSO fără sudură), consultați [Azure Active Directory fără sudură sign-on unic: întrebări frecvente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Pentru informații despre depanarea problemelor comune cu privire la Sign-On Azure Active Directory (Azure AD) fără sudură (SSO fără sudură), consultați [Depanarea conectării unice la Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
