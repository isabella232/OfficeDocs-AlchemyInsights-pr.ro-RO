---
title: Active Directory nu se sincronizează
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265268"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="68855-102">Active Directory nu se sincronizează</span><span class="sxs-lookup"><span data-stu-id="68855-102">Active Directory not syncing</span></span>

<span data-ttu-id="68855-103">Dacă primiți erori de sincronizare, ar fi nici o sincronizare recentă, sau observați starea de sincronizare director în portalul de administrare Office spune, Ultima sincronizat mai mult de 3 zile în urmă, este posibil ca AADConnect are setări incorecte sau insuficiente permisiuni pentru a efectua o sincronizare.</span><span class="sxs-lookup"><span data-stu-id="68855-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="68855-104">Reinstalarea AADConnect utilizând setările expres poate rezolva problema rapid:</span><span class="sxs-lookup"><span data-stu-id="68855-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="68855-105">[Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="68855-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="68855-106">[Urmați instrucțiunile de instalare expres](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="68855-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="68855-107">Pentru mai multe informații despre conturile de serviciu AADConnect, consultați [Azure AD Connect: Conturi și permisiuni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="68855-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
