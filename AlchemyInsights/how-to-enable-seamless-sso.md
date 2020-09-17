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
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="2406d-102">Cum se activează SSO fără sudură</span><span class="sxs-lookup"><span data-stu-id="2406d-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="2406d-103">Activați SSO fără sudură prin [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="2406d-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="2406d-104">Dacă efectuați o instalare nouă de Azure AD Connect, alegeți [calea de instalare particularizată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="2406d-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="2406d-105">În pagina de **conectare a utilizatorului** , alegeți opțiunea **Activare sign-on unic** .</span><span class="sxs-lookup"><span data-stu-id="2406d-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="2406d-106">Pentru a verifica dacă ați activat corect SSO perfect:</span><span class="sxs-lookup"><span data-stu-id="2406d-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="2406d-107">Conectați-vă la [Centrul de administrare Azure Active Directory](https://aad.portal.azure.com) ca administrator global.</span><span class="sxs-lookup"><span data-stu-id="2406d-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="2406d-108">Selectați **Azure Active Directory** în panoul din stânga.</span><span class="sxs-lookup"><span data-stu-id="2406d-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="2406d-109">Verificați dacă este **activat**un singur sign-on fără sudură.</span><span class="sxs-lookup"><span data-stu-id="2406d-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="2406d-110">Pentru a afla mai multe, consultați [Azure Active Directory fără sudură sign-on unic: pornire rapidă](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="2406d-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  