---
title: Imposibil de accesat folderele publice
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959506"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="429be-102">Outlook nu se poate conecta la foldere publice</span><span class="sxs-lookup"><span data-stu-id="429be-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="429be-103">Dacă accesul public folder nu funcționează pentru puțini utilizatori, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="429be-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="429be-104">Conectați-vă la EXO PowerShell și configurați DefaultPublicFolderMailbox pe contul de utilizator problema pentru a se potrivi cu unul pe un cont de utilizator de lucru.</span><span class="sxs-lookup"><span data-stu-id="429be-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="429be-105">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="429be-105">Example:</span></span>

<span data-ttu-id="429be-106">Get-cutie poștală WorkingUser | ft DefaultPublicFolderMailbox, Efectivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="429be-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="429be-107">Set-Mailbox Problemusutilizator-DefaultPublicFolderMailbox \<valoare de la comanda anterioară></span><span class="sxs-lookup"><span data-stu-id="429be-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="429be-108">Așteptați cel puțin o oră pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="429be-108">Wait at least one hour for the change to take effect.</span></span>