---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820190"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="cc1e9-102">Blocarea autentificării moștenite</span><span class="sxs-lookup"><span data-stu-id="cc1e9-102">Blocking legacy authentication</span></span>

<span data-ttu-id="cc1e9-103">Autentificarea moștenit este un termen care se referă la o solicitare de autentificare efectuată de:</span><span class="sxs-lookup"><span data-stu-id="cc1e9-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="cc1e9-104">Clienții Office mai vechi, care nu utilizează autentificarea modernă (de exemplu, clientul Office 2010).</span><span class="sxs-lookup"><span data-stu-id="cc1e9-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="cc1e9-105">Orice client care utilizează protocoale de e-mail moștenite, cum ar fi IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="cc1e9-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="cc1e9-106">Pentru mai multe informații despre blocarea autentificării moștenite și activarea autentificării moderne, consultați Blocarea [autentificării moștenite.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="cc1e9-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="cc1e9-107">Valorile implicite de securitate din Azure Active Directory (Azure AD) simplifică securizarea și protejarea organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="cc1e9-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="cc1e9-108">Setările de securitate implicite conțin setări de securitate preconfigurate pentru atacurile obișnuite.</span><span class="sxs-lookup"><span data-stu-id="cc1e9-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="cc1e9-109">Pentru mai multe informații despre setările implicite de securitate, consultați [Ce sunt valorile implicite de securitate?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="cc1e9-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="cc1e9-110">**Notă:** dacă entitatea dvs. găzduită a fost creată pe 22 octombrie 2019 sau după aceasta, este posibil să vă confruntați cu noul comportament securizat în mod implicit și să aveți deja activată setarea implicită de securitate în entitatea dvs. găzduită.</span><span class="sxs-lookup"><span data-stu-id="cc1e9-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="cc1e9-111">Pentru a ne proteja toți utilizatorii, valorile implicite de securitate sunt create pentru toate entitățile găzduite noi.</span><span class="sxs-lookup"><span data-stu-id="cc1e9-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
