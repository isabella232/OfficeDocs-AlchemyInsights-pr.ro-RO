---
title: Active Directory nu se sincronizează
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822863"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="027e4-102">Active Directory nu se sincronizează</span><span class="sxs-lookup"><span data-stu-id="027e4-102">Active Directory not syncing</span></span>

<span data-ttu-id="027e4-103">Dacă primiți erori de sincronizare, cum ar fi "nicio sincronizare recentă" sau observați starea de sincronizare a directorului în portalul de administrare Office spune "Ultima sincronizare a fost sincronizată în urmă cu mai mult de 3 zile", poate fi faptul că AADConnect are setări incorecte sau permisiuni insuficiente pentru a efectua o sincronizare.</span><span class="sxs-lookup"><span data-stu-id="027e4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="027e4-104">Reinstalarea AADConnect utilizând setări expres poate rezolva rapid problema:</span><span class="sxs-lookup"><span data-stu-id="027e4-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="027e4-105">[Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="027e4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="027e4-106">[Urmați instrucțiunile pentru instalarea expres.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="027e4-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="027e4-107">Pentru mai multe informații despre conturile de serviciu AADConnect, [consultați Azure AD Connect: Conturi și permisiuni.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="027e4-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
