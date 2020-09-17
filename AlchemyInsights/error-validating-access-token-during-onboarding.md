---
title: A apărut o eroare la validarea erorii simbolurilor Access în timpul analizei desktop la îmbarcare
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783563"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="13eec-102">Eroarea "eroare de validare a simbolurilor de acces" în timpul analizei pentru desktop</span><span class="sxs-lookup"><span data-stu-id="13eec-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="13eec-103">Această eroare este observată în mod normal atunci când simbolul de autentificare expiră.</span><span class="sxs-lookup"><span data-stu-id="13eec-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="13eec-104">De obicei, reîmprospătarea paginii reîmprospătează simbolul.</span><span class="sxs-lookup"><span data-stu-id="13eec-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="13eec-105">Cu toate acestea, această problemă poate persista dacă există politici de acces condiționat aplicate contului utilizat la analizele desktop la bord.</span><span class="sxs-lookup"><span data-stu-id="13eec-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="13eec-106">Puteți să examinați jurnalele Azure AD sign in în portalul Azure pentru a vedea dacă există erori de conectare pentru contul utilizat pentru controlul de analiză desktop.</span><span class="sxs-lookup"><span data-stu-id="13eec-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="13eec-107">Pentru mai multe informații despre accesul condiționat, vizitați [Planificarea implementării accesului condiționat](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="13eec-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>