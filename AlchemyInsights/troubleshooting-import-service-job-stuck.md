---
title: Depanarea problemelor legate de serviciul de import blocat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125491"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="4f988-102">Depanarea problemelor legate de serviciul de import blocat</span><span class="sxs-lookup"><span data-stu-id="4f988-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="4f988-103">Dacă aveți probleme cu activitățile de import de serviciu blocate sau care nu reușesc, examinați și încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="4f988-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="4f988-104">Revizuiți dimensiunea fișierului PST.</span><span class="sxs-lookup"><span data-stu-id="4f988-104">Review the size of of the PST file.</span></span> <span data-ttu-id="4f988-105">Dimensiunea maximă recomandată a unui fișier PST pentru import este de 20 GB.</span><span class="sxs-lookup"><span data-stu-id="4f988-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="4f988-106">Dacă suspectați că elementele ignorate din cauza coruperei, Scanpst.exe pentru a diagnostica și a remedia erorile din fișierele PST.</span><span class="sxs-lookup"><span data-stu-id="4f988-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="4f988-107">Dacă vedeți o eroare "MapiExceptionShutoffQuotaExceeded" în timpul importului, asigurați-vă că cutia poștală țintă are suficientă capacitate pentru a importa fișierele PST dorite.</span><span class="sxs-lookup"><span data-stu-id="4f988-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="4f988-108">Pentru mai multe informații despre depanarea problemelor cu activitățile de import PST, consultați [Depanarea problemelor cu activitățile de import PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="4f988-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="4f988-109">Pentru informații despre cum să remediați problemele atunci când importați fișiere PST în Outlook, consultați Remedierea problemelor cu importul unui fișier [.pst Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="4f988-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>