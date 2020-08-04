---
title: Utilizarea înregistrării în jurnal a utilizării pentru Azure Rights Management
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556028"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="5f8be-102">Utilizarea înregistrării în jurnal a utilizării pentru Azure Rights Management</span><span class="sxs-lookup"><span data-stu-id="5f8be-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="5f8be-103">În mod implicit, înregistrarea în jurnal a utilizării protecției este activată pentru toți clienții.</span><span class="sxs-lookup"><span data-stu-id="5f8be-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="5f8be-104">Jurnalele sunt scrise ca o serie de blobs în stocare Azure pentru entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="5f8be-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="5f8be-105">După o acțiune de protecție, poate dura până la 15 minute pentru ca majoritatea jurnalelor să apară.</span><span class="sxs-lookup"><span data-stu-id="5f8be-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="5f8be-106">Aveți posibilitatea să utilizați jurnalele de utilizare a protecției pentru:</span><span class="sxs-lookup"><span data-stu-id="5f8be-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="5f8be-107">Analizați statisticile de afaceri</span><span class="sxs-lookup"><span data-stu-id="5f8be-107">Analyze business insights</span></span>

- <span data-ttu-id="5f8be-108">Monitor pentru abuz</span><span class="sxs-lookup"><span data-stu-id="5f8be-108">Monitor for abuse</span></span>

- <span data-ttu-id="5f8be-109">Efectuarea analizei medico-legale</span><span class="sxs-lookup"><span data-stu-id="5f8be-109">Perform forensic analysis</span></span>

<span data-ttu-id="5f8be-110">Pentru mai multe informații, consultați [Înregistrarea în jurnal și analizarea utilizării protecției din Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="5f8be-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="5f8be-111">Pentru informații despre înregistrarea în jurnal a utilizării clienților, consultați [Ghidul de administrare: Fișierele clientului Azure Information Protection și înregistrarea în jurnal a utilizării clienților](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="5f8be-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="5f8be-112">Pentru informații suplimentare, consultați:</span><span class="sxs-lookup"><span data-stu-id="5f8be-112">For additional information, see:</span></span>

- <span data-ttu-id="5f8be-113">[Cerințe de protecție a informațiilor Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="5f8be-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="5f8be-114">[Tutorial: Configurați setările politicii Azure Information Protection și creați o etichetă nouă](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="5f8be-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>