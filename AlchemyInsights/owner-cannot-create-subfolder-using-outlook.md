---
title: Proprietarul nu poate crea sub folder utilizând Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836147"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="6624d-102">Proprietarul nu poate crea sub folder utilizând Outlook</span><span class="sxs-lookup"><span data-stu-id="6624d-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="6624d-103">**Există o problemă continuă cu proprietarii de foldere publice, care creează subfoldere utilizând Outlook. Problema va fi remediată în curând.**</span><span class="sxs-lookup"><span data-stu-id="6624d-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="6624d-104">Între timp, utilizați una dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="6624d-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="6624d-105">Utilizați Outlook pentru MAC pentru a crea subfolderul, deoarece problema afectează doar Outlook pentru ferestrele desktop (toate versiunile)</span><span class="sxs-lookup"><span data-stu-id="6624d-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="6624d-106">Spuneți administratorului să creeze subfolderul utilizând EXO Shell sau EAC</span><span class="sxs-lookup"><span data-stu-id="6624d-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="6624d-107">Modificați DefaultPublicFolderMailbox/EffectivePublicFolderMailbox a utilizatorului la altă cutie poștală decât cutia poștală de conținut, pentru folderul care provoacă problema</span><span class="sxs-lookup"><span data-stu-id="6624d-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="6624d-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="6624d-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="6624d-109">Așteptați o oră, reporniți clientul Outlook</span><span class="sxs-lookup"><span data-stu-id="6624d-109">Wait for an hour, restart outlook client</span></span>