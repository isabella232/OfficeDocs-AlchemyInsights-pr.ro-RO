---
title: Imposibil de accesat folderele publice
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819524"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="04d8d-102">Outlook nu se poate conecta la folderele publice</span><span class="sxs-lookup"><span data-stu-id="04d8d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="04d8d-103">Dacă accesul la folderele publice nu funcționează pentru unii utilizatori, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="04d8d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="04d8d-104">Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator problemă pentru a se potrivi cu parametrul unui cont de utilizator care lucrează.</span><span class="sxs-lookup"><span data-stu-id="04d8d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="04d8d-105">Exemplu:</span><span class="sxs-lookup"><span data-stu-id="04d8d-105">Example:</span></span>

<span data-ttu-id="04d8d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="04d8d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="04d8d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="04d8d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="04d8d-108">Așteptați cel puțin o oră pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="04d8d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="04d8d-109">Dacă problema rămâne, urmați această procedură pentru [a depana](https://aka.ms/pfcte) problemele de acces la folderele publice utilizând Outlook.</span><span class="sxs-lookup"><span data-stu-id="04d8d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="04d8d-110">**Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:**</span><span class="sxs-lookup"><span data-stu-id="04d8d-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="04d8d-111">Utilizarea Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true sau $false</span><span class="sxs-lookup"><span data-stu-id="04d8d-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="04d8d-112">$true: Permiteți utilizatorilor să acceseze foldere publice în Outlook</span><span class="sxs-lookup"><span data-stu-id="04d8d-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="04d8d-113">$false: Împiedicarea accesului utilizatorilor la folderele publice în Outlook.</span><span class="sxs-lookup"><span data-stu-id="04d8d-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="04d8d-114">Aceasta este valoarea implicită.</span><span class="sxs-lookup"><span data-stu-id="04d8d-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="04d8d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="04d8d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="04d8d-116">**Notă** Această procedură poate controla conexiunile doar cu clienții Outlook pentru desktop pentru Windows.</span><span class="sxs-lookup"><span data-stu-id="04d8d-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="04d8d-117">Un utilizator poate continua să acceseze folderele publice utilizând OWA sau Outlook pentru Mac.</span><span class="sxs-lookup"><span data-stu-id="04d8d-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="04d8d-118">Pentru mai multe informații, [consultați Anunțarea suportului pentru Conexiuni controlate la folderele publice din Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="04d8d-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>