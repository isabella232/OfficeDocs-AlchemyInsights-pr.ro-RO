---
title: Nu puteți accesa folderele publice
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812559"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="05c66-102">Outlook nu se poate conecta la folderele publice</span><span class="sxs-lookup"><span data-stu-id="05c66-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="05c66-103">Dacă accesul la foldere publice nu funcționează pentru unii utilizatori, încercați următoarele:</span><span class="sxs-lookup"><span data-stu-id="05c66-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="05c66-104">Conectați-vă la EXO PowerShell și configurați parametrul DefaultPublicFolderMailbox pe contul de utilizator al problemei pentru a se potrivi cu parametrul pentru un cont de utilizator care funcționează.</span><span class="sxs-lookup"><span data-stu-id="05c66-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="05c66-105">Exemplu</span><span class="sxs-lookup"><span data-stu-id="05c66-105">Example:</span></span>

<span data-ttu-id="05c66-106">WorkingUser de primire a cutiei poștale | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="05c66-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="05c66-107">Set-cutia poștală ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="05c66-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="05c66-108">Așteptați cel puțin o oră pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="05c66-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="05c66-109">Dacă problema rămâne, vă rugăm să urmați [această procedură](https://aka.ms/pfcte) pentru a depana problemele de acces la foldere publice utilizând Outlook.</span><span class="sxs-lookup"><span data-stu-id="05c66-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="05c66-110">**Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook**:</span><span class="sxs-lookup"><span data-stu-id="05c66-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="05c66-111">Utilizați Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True sau $false</span><span class="sxs-lookup"><span data-stu-id="05c66-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="05c66-112">$true: Permiteți utilizatorilor să acceseze folderele publice în Outlook</span><span class="sxs-lookup"><span data-stu-id="05c66-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="05c66-113">$false: împiedicați accesul utilizatorilor la foldere publice în Outlook.</span><span class="sxs-lookup"><span data-stu-id="05c66-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="05c66-114">Aceasta este valoarea implicită.</span><span class="sxs-lookup"><span data-stu-id="05c66-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="05c66-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="05c66-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="05c66-116">**Notă** Această procedură poate controla conexiunile doar cu clienții Outlook desktop pentru Windows.</span><span class="sxs-lookup"><span data-stu-id="05c66-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="05c66-117">Un utilizator poate continua să acceseze foldere publice folosind OWA sau Outlook pentru Mac.</span><span class="sxs-lookup"><span data-stu-id="05c66-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="05c66-118">Pentru mai multe informații, consultați [anunțarea acceptării conexiunilor controlate la foldere publice în Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="05c66-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>