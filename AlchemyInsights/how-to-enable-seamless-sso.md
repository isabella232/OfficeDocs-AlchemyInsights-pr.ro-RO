---
title: Cum se activează SSO fără sudură
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780539"
---
# <a name="how-to-enable-seamless-sso"></a>Cum se activează SSO fără sudură

Activați SSO fără sudură prin [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Dacă efectuați o instalare nouă de Azure AD Connect, alegeți [calea de instalare particularizată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). În pagina de **conectare a utilizatorului** , alegeți opțiunea **Activare sign-on unic** .
  
Pentru a verifica dacă ați activat corect SSO perfect:
  
1. Conectați-vă la [Centrul de administrare Azure Active Directory](https://aad.portal.azure.com) ca administrator global.

2. Selectați **Azure Active Directory** în panoul din stânga.

3. Verificați dacă este **activat**un singur sign-on fără sudură.

Pentru a afla mai multe, consultați [Azure Active Directory fără sudură sign-on unic: pornire rapidă](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  