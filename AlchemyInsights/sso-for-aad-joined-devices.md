---
title: Single-Sign activat pentru dispozitivele la care s-a alăturat Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405658"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Sign-on unic pentru dispozitivele la care s-a alăturat Azure Active Directory

Dacă aveți un mediu Local Active Directory (AD) și doriți să vă asociați computerelor care au domeniul unit cu Azure AD, puteți realiza acest lucru prin asocierea hibridă Azure AD. [Modul către: Planificarea implementării](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) hibride de asociere la Azure Active Directory vă furnizează pașii asociați pentru a implementa o asociere Azure AD hibridă în mediul dvs.

[Configurarea dispozitivelor cu asociere Azure AD pentru dispozitive Single-Sign local utilizând Windows Hello pentru business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme principale cu tokenul de reîmprospătare (PRT)** Un token de reîmprospătare principal (PRT) este un artefact cheie de autentificare Azure AD pe dispozitive Windows 10, Windows Server 2016 și versiuni mai recente, iOS și Android. Este un simbol web JSON (JWT) emis special către tokenul de la prima parte Microsoft, pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe aceste dispozitive. În Ce este un token de reîmprospătare [principal?,](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)vom oferi detalii despre modul în care un PRT este emis, utilizat și protejat pe dispozitivele Windows 10.

**WamDefaultSet: YES și AzureADPrt: DA** Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD atunci când s-a conectat la dispozitiv. Dacă valorile sunt **NU,** este posibil ca aceasta să fie scadentă:

- Cheie de stocare nereparticulară în TPM asociată cu dispozitivul după înregistrare (verificați KeySignTest în timp ce rulează cu nivel ridicat).
- ID conectare alternativă
- Proxy HTTP nu a fost găsit

Depanarea dispozitivelor utilizând comanda dsregcmd - [starea SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
