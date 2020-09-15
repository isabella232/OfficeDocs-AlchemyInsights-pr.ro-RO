---
title: Active Directory nu se sincronizează
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697641"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="cb86b-102">Active Directory nu se sincronizează</span><span class="sxs-lookup"><span data-stu-id="cb86b-102">Active Directory not syncing</span></span>

<span data-ttu-id="cb86b-103">Dacă primiți erori de sincronizare, cum ar fi "fără sincronizare recentă" sau observați starea de sincronizare a directorului în portalul de administrare Office spune "Ultima sincronizare cu mai mult de 3 zile în urmă", este posibil ca AADConnect să aibă setări incorecte sau permisiuni insuficiente pentru a efectua o sincronizare.</span><span class="sxs-lookup"><span data-stu-id="cb86b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="cb86b-104">Reinstalarea AADConnect utilizând setările expres poate rezolva rapid problema:</span><span class="sxs-lookup"><span data-stu-id="cb86b-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="cb86b-105">[Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="cb86b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="cb86b-106">[Urmați instrucțiunile pentru instalarea expres](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="cb86b-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="cb86b-107">Pentru mai multe informații despre conturile de serviciu AADConnect, consultați [AZURE AD Connect: conturi și permisiuni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="cb86b-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
