---
title: Imposibil de șters elementele din SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511988"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f33c2-102">Imposibil de șters elemente</span><span class="sxs-lookup"><span data-stu-id="f33c2-102">Unable to delete items</span></span>

<span data-ttu-id="f33c2-103">Politicile de conservare poate provoca acest lucru, trebuie să dezactivați sau exclude țirea respectivă care cauzează această problemă.</span><span class="sxs-lookup"><span data-stu-id="f33c2-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f33c2-104">După ce o politică de conservare sau de așteptare este eliminat, poate dura până la 24 de ore pentru ca modificarea să intre în vigoare.</span><span class="sxs-lookup"><span data-stu-id="f33c2-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="f33c2-105">Asigurați-vă că nu există o [configurare a politicii](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) de conservare pe element.</span><span class="sxs-lookup"><span data-stu-id="f33c2-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="f33c2-106">Este posibil ca site-ul să fi depășit limita de stocare, să mărească [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.</span><span class="sxs-lookup"><span data-stu-id="f33c2-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="f33c2-107">Asigurați-vă că elementul nu este [extras la](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) un alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="f33c2-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="f33c2-108">În cele din urmă, administratorii pot utiliza [Modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni complexe de gestionare, ar fi eliminarea forțată elemente încăpățânate.</span><span class="sxs-lookup"><span data-stu-id="f33c2-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f33c2-109">Eliminare fișier PNP</span><span class="sxs-lookup"><span data-stu-id="f33c2-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f33c2-110">Eliminare folder PNP</span><span class="sxs-lookup"><span data-stu-id="f33c2-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f33c2-111">Eliminare element listă PNP</span><span class="sxs-lookup"><span data-stu-id="f33c2-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f33c2-112">Eliminare listă PNP</span><span class="sxs-lookup"><span data-stu-id="f33c2-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f33c2-113">Eliminare câmp PNP (coloană)</span><span class="sxs-lookup"><span data-stu-id="f33c2-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)