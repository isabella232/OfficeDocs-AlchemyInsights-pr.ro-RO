---
title: Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714978"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="a5e86-102">Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple</span><span class="sxs-lookup"><span data-stu-id="a5e86-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="a5e86-103">"Am detectat că aveți unul sau mai multe simboluri ADE/DEP care se află într-o stare de eroare.</span><span class="sxs-lookup"><span data-stu-id="a5e86-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="a5e86-104">Până când starea erorii este rezolvată pentru fiecare simbol afectat, funcționalitatea ADE nu va funcționa la fel ".</span><span class="sxs-lookup"><span data-stu-id="a5e86-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="a5e86-105">Această eroare s-ar putea manifesta în mai multe moduri, inclusiv:</span><span class="sxs-lookup"><span data-stu-id="a5e86-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="a5e86-106">Este posibil ca dispozitivele să nu se sincronizeze de la ABM/ASM la Intune</span><span class="sxs-lookup"><span data-stu-id="a5e86-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="a5e86-107">Atribuirile de profil de înscriere pot fi nereușite</span><span class="sxs-lookup"><span data-stu-id="a5e86-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="a5e86-108">Este posibil ca dispozitivele să nu finalizeze cu succes înscrierea ADE</span><span class="sxs-lookup"><span data-stu-id="a5e86-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="a5e86-109">Verificați dacă eroarea de sincronizare a fost raportată în consola Intune de sub **dispozitive > Înscrieți dispozitivele > înscriere Apple > tokenuri de program de înscriere** și revizuiți următoarea documentație pentru a vedea orice remediere potențială:</span><span class="sxs-lookup"><span data-stu-id="a5e86-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="a5e86-110">Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS</span><span class="sxs-lookup"><span data-stu-id="a5e86-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
