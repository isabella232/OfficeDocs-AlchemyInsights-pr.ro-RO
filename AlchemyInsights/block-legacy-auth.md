---
title: BlockLegacyAuth (În)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079272"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="83a5b-102">Blocarea autentificării moștenite</span><span class="sxs-lookup"><span data-stu-id="83a5b-102">Blocking legacy authentication</span></span>

<span data-ttu-id="83a5b-103">Autentificarea moștenită este un termen care se referă la o solicitare de autentificare făcută de:</span><span class="sxs-lookup"><span data-stu-id="83a5b-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="83a5b-104">Clienții Office mai vechi care nu utilizează autentificarea modernă (de exemplu, clientul Office 2010).</span><span class="sxs-lookup"><span data-stu-id="83a5b-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="83a5b-105">Orice client care utilizează protocoale de poștă electronică moștenite, ar fi IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="83a5b-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="83a5b-106">Pentru mai multe informații despre blocarea autentificării moștenite și activarea autentificării moderne, consultați [Blocarea autentificării moștenite](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="83a5b-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="83a5b-107">Valorile implicite de securitate din Azure Active Directory (Azure AD) facilitează securizarea și protejarea organizației.</span><span class="sxs-lookup"><span data-stu-id="83a5b-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="83a5b-108">Valorile implicite de securitate conțin setări de securitate preconfigurate pentru atacuri lecomune.</span><span class="sxs-lookup"><span data-stu-id="83a5b-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="83a5b-109">Pentru mai multe informații despre valorile implicite de securitate, consultați [Ce sunt valorile implicite de securitate?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="83a5b-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="83a5b-110">**Notă:** Dacă entitatea găzduită a fost creată la sau după 22 octombrie 2019, este posibil să vă confruntați cu noul comportament sigur în mod implicit și aveți deja valorile implicite de securitate activate în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="83a5b-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="83a5b-111">Într-un efort de a proteja toți utilizatorii noștri, valorile implicite de securitate sunt implementate pentru toți chiriașii noi creați.</span><span class="sxs-lookup"><span data-stu-id="83a5b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
