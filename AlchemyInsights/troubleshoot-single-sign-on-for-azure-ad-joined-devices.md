---
title: Depanarea sign-on unic pentru dispozitivele cu Asociere Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039258"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Depanarea sign-on unic pentru dispozitivele cu Asociere Azure AD

Dacă aveți un mediu Local Active Directory (AD) și doriți să vă asociați computerelor care au domeniul unit cu Azure AD, puteți realiza acest lucru prin asocierea hibridă Azure AD. [Cum să: Planificați implementarea hibridă a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) de asociere vă furnizează pașii asociați pentru a implementa o asociere Azure AD hibridă în mediul dvs.

Pentru mai multe informații, consultați Configurarea dispozitivelor cu asociere Azure AD pentru dispozitive [Single-Sign Pe utilizând Windows Hello pentru business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Probleme principale cu tokenul de reîmprospătare (PRT)**

Un token de reîmprospătare primară (PRT) este un artefact cheie de autentificare Azure AD pe dispozitive Windows 10, Windows Server 2016 și versiuni mai recente, iOS și Android. Este un simbol web JSON (JWT) emis special către tokenul de la prima parte Microsoft, pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe aceste dispozitive. Pentru detalii despre modul în care este emis, utilizat și protejat un PRT pe Windows 10 dispozitive, consultați Ce este un token [de reîmprospătare principal?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES și AzureADPrt: DA**

Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD atunci când s-a conectat la dispozitiv. Dacă valorile sunt **NU,** cauza poate fi:

- Cheie de stocare nereparticulară în TPM asociată cu dispozitivul după înregistrare (verificați KeySignTest în timp ce rulează cu nivel mare)
- ID conectare alternativă
- Proxy HTTP nu a fost găsit

Pentru a depana dispozitivele utilizând comanda dsregcmd, consultați [Starea SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
