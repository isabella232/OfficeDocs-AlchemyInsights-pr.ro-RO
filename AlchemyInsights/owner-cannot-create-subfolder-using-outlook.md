---
title: Proprietarul nu poate crea subfolder utilizând Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665730"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="393e6-102">Proprietarul nu poate crea subfolder utilizând Outlook</span><span class="sxs-lookup"><span data-stu-id="393e6-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="393e6-103">**Există o problemă în curs de desfășurare cu proprietarii de foldere publice care creează subfoldere utilizând Outlook. Problema va fi remediată în curând.**</span><span class="sxs-lookup"><span data-stu-id="393e6-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="393e6-104">Între timp, utilizați una dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="393e6-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="393e6-105">Utilizați Outlook pentru MAC pentru a crea subfolderul ca problema afectează numai Outlook pentru desktop Windows (toate versiunile)</span><span class="sxs-lookup"><span data-stu-id="393e6-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="393e6-106">Administratorul să creeze subfolderul utilizând EXO Shell sau EAC</span><span class="sxs-lookup"><span data-stu-id="393e6-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="393e6-107">Modificarea DefaultPublicFolderMailbox/EffectivePublicFolderMailbox pentru utilizator în altă cutie poștală decât cutia poștală de conținut pentru folderul care cauzează problema</span><span class="sxs-lookup"><span data-stu-id="393e6-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="393e6-108">*Set-cutia poștală user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="393e6-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="393e6-109">Așteptați o oră, reporniți clientul Outlook</span><span class="sxs-lookup"><span data-stu-id="393e6-109">Wait for an hour, restart outlook client</span></span>