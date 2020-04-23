---
title: Restricționarea SharePoint Online la modul clasic
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742481"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9bb5f-102">Restricționarea SharePoint Online la modul clasic</span><span class="sxs-lookup"><span data-stu-id="9bb5f-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9bb5f-103">Unele organizații necesită în continuare experiența modului clasic.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9bb5f-104">Deși nu există planuri de eliminare a modului clasic la un nivel granular, nu mai este posibil să restricționați o întreagă organizație (entitate găzduită) la modul clasic pentru liste și biblioteci.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9bb5f-105">Administratorul va avea următoarele opțiuni pentru a gestiona listele și bibliotecile individuale în modul clasic utilizând comutatoare de renunțare granulare pe care le oferim la următoarele niveluri:</span><span class="sxs-lookup"><span data-stu-id="9bb5f-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9bb5f-106">colecție de site-uri</span><span class="sxs-lookup"><span data-stu-id="9bb5f-106">site collection</span></span>
- <span data-ttu-id="9bb5f-107">Site</span><span class="sxs-lookup"><span data-stu-id="9bb5f-107">site</span></span>
- <span data-ttu-id="9bb5f-108">Listă</span><span class="sxs-lookup"><span data-stu-id="9bb5f-108">list</span></span>
- <span data-ttu-id="9bb5f-109">Biblioteca</span><span class="sxs-lookup"><span data-stu-id="9bb5f-109">library</span></span>

<span data-ttu-id="9bb5f-110">În plus, listele care utilizează anumite caracteristici și particularizări care nu sunt acceptate de modern va fi în continuare automat comutate la modul clasic.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9bb5f-111">Începând cu 1 aprilie 2019, procesul de dezactivare a nivelului de entitate găzduită renunță la lista modernă, iar bibliotecile vor începe și vor continua până la 31 mai 2019.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="9bb5f-112">Listele și bibliotecile care se află în modul clasic ca urmare a excluderii pentru entitate găzduită vor fi mutate automat la modern.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="9bb5f-113">Dacă aveți nevoie de modul clasic, vă rugăm să consultați mai multe informații [aici](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) și instrucțiuni Powershell PnP [aici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) care descrie opțiunile și instrumentele pe care le puteți utiliza astăzi pentru a utiliza experiența modului clasic.</span><span class="sxs-lookup"><span data-stu-id="9bb5f-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
