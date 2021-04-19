---
title: Controlul accesului la folderele publice utilizând Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816752"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="9d2e8-102">Controlul accesului la folderele publice utilizând Outlook</span><span class="sxs-lookup"><span data-stu-id="9d2e8-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="9d2e8-103">Pentru a controla ce utilizatori pot accesa folderele publice utilizând Outlook:</span><span class="sxs-lookup"><span data-stu-id="9d2e8-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="9d2e8-104">Utilizare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="9d2e8-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="9d2e8-105">$true: Permiteți utilizatorilor să acceseze foldere publice în Outlook</span><span class="sxs-lookup"><span data-stu-id="9d2e8-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="9d2e8-106">$false: Împiedicarea accesului utilizatorilor la folderele publice în Outlook.</span><span class="sxs-lookup"><span data-stu-id="9d2e8-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="9d2e8-107">Aceasta este valoarea implicită.</span><span class="sxs-lookup"><span data-stu-id="9d2e8-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="9d2e8-108">Notă: Această procedură poate controla doar conexiunile cu clienții Outlook pentru desktop pentru Windows.</span><span class="sxs-lookup"><span data-stu-id="9d2e8-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="9d2e8-109">Utilizatorii pot continua să acceseze foldere publice utilizând OWA sau Outlook pentru Mac.</span><span class="sxs-lookup"><span data-stu-id="9d2e8-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="9d2e8-110">Pentru mai multe informații, [consultați Conexiuni controlate la folderele publice din Outlook pentru](https://aka.ms/controlpf) mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="9d2e8-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
