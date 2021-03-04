---
title: Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448934"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="ce07b-102">Erorile de sincronizare pentru înregistrare automată a dispozitivelor Apple</span><span class="sxs-lookup"><span data-stu-id="ce07b-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="ce07b-103">"Am detectat că aveți unul sau mai multe simboluri ADE/DEP care se află într-o stare de eroare.</span><span class="sxs-lookup"><span data-stu-id="ce07b-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="ce07b-104">Până când starea erorii este rezolvată pentru fiecare simbol afectat, funcționalitatea ADE nu va funcționa așa cum vă așteptați. ".</span><span class="sxs-lookup"><span data-stu-id="ce07b-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="ce07b-105">Această eroare s-ar putea manifesta în mai multe moduri, inclusiv:</span><span class="sxs-lookup"><span data-stu-id="ce07b-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="ce07b-106">Este posibil ca dispozitivele să nu se sincronizeze de la ABM/ASM la Intune</span><span class="sxs-lookup"><span data-stu-id="ce07b-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="ce07b-107">Atribuirile de profil de înscriere pot fi nereușite</span><span class="sxs-lookup"><span data-stu-id="ce07b-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="ce07b-108">Este posibil ca dispozitivele să nu finalizeze cu succes înscrierea ADE</span><span class="sxs-lookup"><span data-stu-id="ce07b-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="ce07b-109">Verificați dacă eroarea de sincronizare a fost raportată în consola Intune de sub **dispozitive > Înscrieți dispozitivele > înscriere Apple > token**-ul programului de înscriere.</span><span class="sxs-lookup"><span data-stu-id="ce07b-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="ce07b-110">Una dintre cele mai comune cauze ale erorii de sincronizare este expirarea simbolului curent.</span><span class="sxs-lookup"><span data-stu-id="ce07b-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="ce07b-111">În multe cazuri, reînnoirea simbolului afectat va rezolva problema.</span><span class="sxs-lookup"><span data-stu-id="ce07b-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="ce07b-112">Dacă una sau mai multe dintre jetoane a expirat, consultați următoarea documentație pentru a vă ajuta să le reînnoiți, după cum este necesar:</span><span class="sxs-lookup"><span data-stu-id="ce07b-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="ce07b-113">Reînnoirea unui simbol de înscriere automată a dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="ce07b-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="ce07b-114">În plus, puteți vedea următoarea documentație pentru a vedea potențialele remedieri pentru alte erori care cauzează erorile de sincronizare a tokenului:</span><span class="sxs-lookup"><span data-stu-id="ce07b-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="ce07b-115">Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS</span><span class="sxs-lookup"><span data-stu-id="ce07b-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="ce07b-116">Erorile de sincronizare ABM/ASM pentru token-ul de înscriere a dispozitivelor automate pentru iOS/iPadOS și macOS</span><span class="sxs-lookup"><span data-stu-id="ce07b-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
