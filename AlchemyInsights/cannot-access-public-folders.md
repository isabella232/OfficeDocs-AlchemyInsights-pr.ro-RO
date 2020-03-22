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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891761"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4c4cd-102">Outlook nu se poate conecta la foldere publice</span><span class="sxs-lookup"><span data-stu-id="4c4cd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4c4cd-103">Dacă accesul la foldere publice nu funcționează pentru unii utilizatori, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="4c4cd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="4c4cd-104">Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator problemă pentru a se potrivi parametrului pe un cont de utilizator de lucru.</span><span class="sxs-lookup"><span data-stu-id="4c4cd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="4c4cd-105">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="4c4cd-105">Example:</span></span>

<span data-ttu-id="4c4cd-106">Ia-Cutie poștală WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="4c4cd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4c4cd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<valoare din comanda anterioară></span><span class="sxs-lookup"><span data-stu-id="4c4cd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4c4cd-108">Așteptați cel puțin o oră pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="4c4cd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="4c4cd-109">Dacă problema rămâne, urmați [această procedură](https://aka.ms/pfcte) pentru a depana problemele de acces la folderele publice utilizând Outlook.</span><span class="sxs-lookup"><span data-stu-id="4c4cd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>