---
title: Eroare la validarea accesării simbolului de acces pe desktop Analytics la îmbarcare
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741250"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="f518a-102">"A existat o eroare de validare a simbolului de acces" eroare în timpul desktop Analytics punerea</span><span class="sxs-lookup"><span data-stu-id="f518a-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="f518a-103">Această eroare se observă în mod normal atunci când expiră simbolul de autentificare.</span><span class="sxs-lookup"><span data-stu-id="f518a-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="f518a-104">De obicei, reîmprospătarea paginii reîmprospătează simbolul.</span><span class="sxs-lookup"><span data-stu-id="f518a-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="f518a-105">Cu toate acestea, această problemă poate persista dacă există orice politici de acces condiționat aplicate la contul utilizat la bord desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="f518a-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="f518a-106">Aveți posibilitatea să examinați jurnalele de autentificare Azure AD în portalul Azure pentru a vedea dacă există erori de sign in pentru contul utilizat pentru desktop Analytics onboarding.</span><span class="sxs-lookup"><span data-stu-id="f518a-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="f518a-107">Pentru mai multe informații despre acces condiționat, vizitați [planul de implementare condițională de acces](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="f518a-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>