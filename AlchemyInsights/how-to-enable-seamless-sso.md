---
title: se activează SSO fără sudură
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "36663884"
---
# <a name="how-to-enable-seamless-sso"></a>se activează SSO fără sudură

Activați SSO fără sudură prin [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Dacă faceți o instalare nouă de Azure AD Connect, alegeți calea de [instalare particularizată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). În pagina **De conectare utilizator,** alegeți opțiunea **Activare sign-on unic.**
  
Pentru a verifica dacă ați activat SSO fără sudură corect:
  
1. Conectați-vă la [centrul administrativ Azure Active Directory](https://aad.portal.azure.com) ca administrator global.

2. Selectați **Azure Active Directory** în panoul din stânga.

3. Verificați dacă este **activată**conectarea unică fără probleme .

Pentru a afla mai multe, consultați [Azure Active Directory Fără sudură Singur Sign-On: Pornire rapidă](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  