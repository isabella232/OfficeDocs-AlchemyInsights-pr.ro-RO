---
title: Imposibil de șters elemente în SharePoint sau OneDrive
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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049529"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e88a2-102">Imposibil de șters elemente</span><span class="sxs-lookup"><span data-stu-id="e88a2-102">Unable to delete items</span></span>

<span data-ttu-id="e88a2-103">Probleme la ștergerea elementelor SharePoint?</span><span class="sxs-lookup"><span data-stu-id="e88a2-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="e88a2-104">Asigurați-vă întotdeauna că aveți [permisiunile corespunzătoare](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) pentru a șterge elementul sau aveți un [administrator de colecție de site-ul](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) încearcă să eliminați elementul.</span><span class="sxs-lookup"><span data-stu-id="e88a2-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="e88a2-105">Asigurați-vă că nu există o setare de [politică de retenție](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pe element.</span><span class="sxs-lookup"><span data-stu-id="e88a2-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="e88a2-106">Asigurați-vă că elementul nu este [verificat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) la un alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="e88a2-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="e88a2-107">În cele din urmă, administratorii pot utiliza [modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni complexe de gestionare, ar fi forța ștergerea elemente încăpățânate.</span><span class="sxs-lookup"><span data-stu-id="e88a2-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e88a2-108">Eliminare fișier PNP</span><span class="sxs-lookup"><span data-stu-id="e88a2-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e88a2-109">Eliminare folder PNP</span><span class="sxs-lookup"><span data-stu-id="e88a2-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e88a2-110">Eliminare element listă PNP</span><span class="sxs-lookup"><span data-stu-id="e88a2-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e88a2-111">Eliminare listă PNP</span><span class="sxs-lookup"><span data-stu-id="e88a2-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e88a2-112">Eliminare câmp PNP (coloană)</span><span class="sxs-lookup"><span data-stu-id="e88a2-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)