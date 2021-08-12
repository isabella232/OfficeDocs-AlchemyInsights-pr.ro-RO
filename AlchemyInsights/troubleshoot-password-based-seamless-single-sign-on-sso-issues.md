---
title: Depanarea problemelor de sign-on unic (SSO) bazate pe parolă
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972836"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Depanarea problemelor de sign-on unic (SSO) bazate pe parolă

Pentru a afla bazele de bază ale SSO bazate pe parolă, consultați [Autentificarea bazată pe parolă cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurarea SSO bazat pe parolă**

1. [Configurarea sign-onului unic bazat pe](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) parolă - Acest articol merge în mai multe detalii despre opțiunea SSO bazată pe parolă. Dacă aplicația pe care o adăugați necesită o configurare particularizată și trebuie să utilizați un SSO bazat pe parolă, acest articol este pentru dvs.
2. [Configurarea semnului unic bazat pe parolă pentru aplicațiile on-prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Proxy aplicație acceptă mai multe moduri de sign-on unic. Sign-onul bazat pe parolă este destinat aplicațiilor care utilizează o combinație nume de utilizator/parolă pentru autentificare. Atunci când configurați sign-on bazat pe parolă pentru aplicația dvs., utilizatorii dvs. trebuie să se conecteze la aplicația local o dată. După aceea, Azure Active Directory stochează informațiile de conectare și le furnizează automat aplicației atunci când utilizatorii dvs. o accesează de la distanță.
    - Ar fi trebuit deja să publicați și să testați aplicația cu Proxy de aplicație. Dacă nu, urmați pașii din Publicați aplicații utilizând proxy-ul de aplicație [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) apoi continuați configurarea SSO bazat pe parolă pentru aplicațiile on-prem.

Pentru a depana SSO bazat pe parolă, [consultați Depanarea sign-onului](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) unic bazat pe parolă în Azure AD
