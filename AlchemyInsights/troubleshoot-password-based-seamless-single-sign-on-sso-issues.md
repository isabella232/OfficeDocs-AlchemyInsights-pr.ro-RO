---
title: Depanarea problemelor cu sign-on unic (SSO) bazate pe parole
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714884"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Depanarea problemelor cu sign-on unic (SSO) bazate pe parole

Pentru a afla fundamentele SSO bazat pe parole, consultați [autentificarea bazată pe parolă cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurarea SSO bazat pe parole**

1. [Configurați sign-on unic bazat pe parolă](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -acest articol intră în mai multe detalii despre opțiunea SSO bazat pe parolă. Dacă aplicația pe care o adăugați necesită configurare particularizată și trebuie să utilizați SSO bazat pe parole, acest articol este pentru dvs.
2. [Configurarea unui singur semn bazat pe parolă pentru aplicațiile on-Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -proxy-ul aplicației acceptă mai multe moduri de sign-on unic. Sign-on bazat pe parolă este destinat aplicațiilor care utilizează o combinație de nume de utilizator/parolă pentru autentificare. Atunci când configurați sign-on bazat pe parolă pentru aplicație, utilizatorii trebuie să se conecteze o dată la aplicația locală. După aceea, Azure Active Directory stochează informațiile de conectare și le furnizează automat aplicației atunci când utilizatorii îl accesează de la distanță.
    - Ar fi trebuit să aveți deja publicat și testat aplicația cu proxy de aplicație. Dacă nu, urmați pașii din [publicarea aplicațiilor folosind proxy-ul aplicației AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , apoi continuați configurația SSO bazat pe parole pentru aplicațiile on-Prem.

Pentru a depana SSO bazat pe parole, consultați [Depanarea conectării unice bazate pe parolă în AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
