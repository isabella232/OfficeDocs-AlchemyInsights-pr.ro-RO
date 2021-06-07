---
title: Probleme de performanță pentru Microsoft Defender pentru punct final în Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794000"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="444e0-102">Probleme de performanță pentru Microsoft Defender pentru punct final în Linux</span><span class="sxs-lookup"><span data-stu-id="444e0-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="444e0-103">Acest articol vă îndrumă prin pașii de identificare a problemelor de performanță pentru Microsoft Defender pentru punct final pe Linux.</span><span class="sxs-lookup"><span data-stu-id="444e0-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="444e0-104">Este important să verificați mai întâi dacă problema cu care vă confruntați se rezolvă cu cea mai [recentă versiune](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="444e0-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="444e0-105">Pentru a începe investigarea, consultați [Depanarea problemelor de performanță pentru Microsoft Defender pentru punct final pe Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="444e0-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="444e0-106">Excluderi</span><span class="sxs-lookup"><span data-stu-id="444e0-106">Exclusions</span></span>

<span data-ttu-id="444e0-107">Excluderile pot contribui la atenuarea problemelor de performanță.</span><span class="sxs-lookup"><span data-stu-id="444e0-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="444e0-108">Revizuiți excluderile înainte de a începe, astfel încât orice risc suplimentar să fie cunoscut și documentat.</span><span class="sxs-lookup"><span data-stu-id="444e0-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="444e0-109">Pentru mai multe informații, consultați [Configurarea și validarea excluderilor pentru Microsoft Defender pentru punctul final pe Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="444e0-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="444e0-110">Atunci când aveți mai multe fișiere & foldere de exclus și toate se rezidă în același loc, ar putea fi mai ușor să excludeți muntele.</span><span class="sxs-lookup"><span data-stu-id="444e0-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="444e0-111">Începând cu lansarea din februarie 101.22.80, puteți exclude un punct de munte întreg.</span><span class="sxs-lookup"><span data-stu-id="444e0-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="444e0-112">De exemplu, dacă /mnt/backup este un punct de munte, puteți adăuga /mnt/backup la lista de excluderi rulezând această comandă:</span><span class="sxs-lookup"><span data-stu-id="444e0-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="444e0-113">**Notă:** Adăugarea excluderilor mărește riscul de detectare a malware-ului și ar trebui gestionat și implementat cu grijă.</span><span class="sxs-lookup"><span data-stu-id="444e0-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="444e0-114">Aveți nevoie de ajutor?</span><span class="sxs-lookup"><span data-stu-id="444e0-114">Need Help?</span></span>

<span data-ttu-id="444e0-115">Pentru a vă asista în modul cel mai eficient, colectați datele de diagnosticare înainte de a deschide un caz de asistență.</span><span class="sxs-lookup"><span data-stu-id="444e0-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
