---
title: Single-Sign pentru toate Azure Active Directory dispozitivele la care s-a făcut asocierea
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050022"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Sign-on unic pentru Azure Active Directory dispozitive cu care s-a făcut asocierea

Dacă aveți un mediu Local Active Directory (AD) și doriți să vă asociați computerelor care au domeniul unit cu Azure AD, puteți realiza acest lucru prin asocierea hibridă Azure AD. [Cum să: Planificați implementarea hibridă a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) de asociere vă furnizează pașii asociați pentru a implementa o asociere Azure AD hibridă în mediul dvs.

[Configurarea dispozitivelor cu asociere Azure AD pentru a le Single-Sign local utilizând Windows Hello pentru business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme principale cu tokenul de reîmprospătare (PRT)** Un token de reîmprospătare primară (PRT) este un artefact cheie de autentificare Azure AD pe dispozitive Windows 10, Windows Server 2016 și versiuni mai recente, iOS și Android. Este un simbol web JSON (JWT) emis special către tokenul de la prima parte Microsoft, pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe aceste dispozitive. În Ce este un token de reîmprospătare [principal?,](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)vom oferi detalii despre modul în care un PRT este emis, utilizat și protejat pe Windows 10 dispozitive.

**WamDefaultSet: YES și AzureADPrt: DA** Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD atunci când s-a conectat la dispozitiv. Dacă valorile sunt **NU,** este posibil ca aceasta să fie scadentă:

- Cheie de stocare nereparticulară în TPM asociată cu dispozitivul după înregistrare (verificați KeySignTest în timp ce rulează cu nivel ridicat).
- ID conectare alternativă
- Proxy HTTP nu a fost găsit

Depanarea dispozitivelor utilizând comanda dsregcmd - [starea SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
