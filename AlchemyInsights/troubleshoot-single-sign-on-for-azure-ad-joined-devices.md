---
title: Depanarea unui singur semn activat pentru dispozitivele Azure AD asociate
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037330"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Depanarea unui singur semn activat pentru dispozitivele Azure AD asociate

Dacă aveți un mediu Active Directory (AD) local și doriți să vă asociați la computerele asociate domeniului de publicitate la Azure AD, puteți realiza acest lucru efectuând asocierea hibrid Azure AD. Instrucțiuni [: planificarea implementării hibride Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vă oferă pașii asociați pentru a implementa un hibrid Azure AD Join în mediul dvs.

Pentru mai multe informații, consultați [Configurarea dispozitivelor asociate AZURE AD pentru Single-Sign local la utilizarea Windows Hello pentru Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Probleme principale de refresh token (PRT)**

Un simbol reîmprospătare principală (PRT) este un artefact cheie al autentificării Azure AD pe Windows 10, Windows Server 2016 și versiunile mai recente, iOS și dispozitivele Android. Acesta este un token web JSON (JWT) emis special pentru brokerii de simboluri pentru prima parte din Microsoft pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe acele dispozitive. Pentru detalii despre modul în care este emis un PRT, utilizat și protejat pe dispozitivele Windows 10, consultați [ce este un token de reîmprospătare primară?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: Da și AzureADPrt: Da**

Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD la conectarea la dispozitiv. Dacă valorile **nu** sunt, se poate datora:

- Cheie de stocare nepotrivită din TPM asociată dispozitivului la înregistrare (Verificați KeySignTest în timp ce lucrați cu ridicat)
- ID de conectare alternativă
- Proxy HTTP negăsit

Pentru a depana dispozitivele utilizând comanda dsregcmd, consultați [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
