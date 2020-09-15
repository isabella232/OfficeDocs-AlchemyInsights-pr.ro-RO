---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685610"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="06973-102">Blocarea autentificării moștenite</span><span class="sxs-lookup"><span data-stu-id="06973-102">Blocking legacy authentication</span></span>

<span data-ttu-id="06973-103">Autentificarea moștenită este un termen care face referire la o solicitare de autentificare efectuată de:</span><span class="sxs-lookup"><span data-stu-id="06973-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="06973-104">Clienții Office mai vechi care nu utilizează autentificarea modernă (de exemplu, clientul Office 2010).</span><span class="sxs-lookup"><span data-stu-id="06973-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="06973-105">Orice client care utilizează protocoale de corespondență moștenite, cum ar fi IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="06973-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="06973-106">Pentru mai multe informații despre blocarea autentificării moștenite și activarea autentificării moderne, consultați [blocarea autentificării moștenite](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="06973-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="06973-107">Setările implicite de securitate din Azure Active Directory (Azure AD) vă ajută să fiți mai ușor de securizat și să contribuiți la protejarea organizației.</span><span class="sxs-lookup"><span data-stu-id="06973-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="06973-108">Setările implicite de securitate conțin setări de securitate preconfigurate pentru atacuri comune.</span><span class="sxs-lookup"><span data-stu-id="06973-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="06973-109">Pentru mai multe informații despre setările implicite de securitate, consultați [ce sunt valorile implicite de securitate?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="06973-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="06973-110">**Notă**: Dacă entitatea găzduită a fost creată la sau după 22 octombrie, 2019, este posibil să întâmpinați noul comportament securizat și aveți deja activate valorile implicite de securitate în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="06973-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="06973-111">Într-un efort de a proteja toți utilizatorii, valorile implicite de securitate sunt derulate pentru toate entitățile găzduite noi create.</span><span class="sxs-lookup"><span data-stu-id="06973-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
