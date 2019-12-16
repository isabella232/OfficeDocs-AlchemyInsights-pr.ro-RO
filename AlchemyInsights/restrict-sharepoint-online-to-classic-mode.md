---
title: Restricționați SharePoint Online la modul clasic
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048772"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="eaaef-102">Restricționați SharePoint Online la modul clasic</span><span class="sxs-lookup"><span data-stu-id="eaaef-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="eaaef-103">Unele organizații necesită încă experiența modul clasic.</span><span class="sxs-lookup"><span data-stu-id="eaaef-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="eaaef-104">Deși nu există planuri pentru a elimina modul clasic la un nivel granulare, nu mai este posibil să se limiteze o organizație întreagă (entitate găzduită) la modul clasic pentru liste și biblioteci.</span><span class="sxs-lookup"><span data-stu-id="eaaef-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="eaaef-105">Administratorul va avea următoarele opțiuni pentru a gestiona listele individuale și bibliotecile în modul clasic folosind switch-uri de opt-out granulare pe care le oferim la următoarele niveluri:</span><span class="sxs-lookup"><span data-stu-id="eaaef-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="eaaef-106">colecție de site-uri</span><span class="sxs-lookup"><span data-stu-id="eaaef-106">site collection</span></span>
- <span data-ttu-id="eaaef-107">Site</span><span class="sxs-lookup"><span data-stu-id="eaaef-107">site</span></span>
- <span data-ttu-id="eaaef-108">Listă</span><span class="sxs-lookup"><span data-stu-id="eaaef-108">list</span></span>
- <span data-ttu-id="eaaef-109">Biblioteca</span><span class="sxs-lookup"><span data-stu-id="eaaef-109">library</span></span>

<span data-ttu-id="eaaef-110">În plus, listele care utilizează anumite caracteristici și particularizări care nu sunt acceptate de modern vor fi în continuare automat comutate la modul clasic.</span><span class="sxs-lookup"><span data-stu-id="eaaef-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="eaaef-111">Începând cu 1 aprilie, 2019, procesul de dezactivare a chiriașului nivel de opt din lista modernă și biblioteci va începe și de a continua prin mai 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="eaaef-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="eaaef-112">Listele și bibliotecile care sunt în modul clasic ca urmare a renunțare la chiriaș vor fi transferate automat la modern.</span><span class="sxs-lookup"><span data-stu-id="eaaef-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="eaaef-113">Dacă aveți nevoie de modul clasic, vă rugăm să vedeți mai multe informații [aici](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) și instrucțiuni PNP PowerShell [aici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) care descrie opțiunile și instrumentele pe care le puteți utiliza astăzi pentru a utiliza experiența modul clasic.</span><span class="sxs-lookup"><span data-stu-id="eaaef-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
