---
title: Imposibil de șters elemente în SharePoint sau OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748588"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="76de5-102">Imposibil de șters elemente</span><span class="sxs-lookup"><span data-stu-id="76de5-102">Unable to delete items</span></span>

<span data-ttu-id="76de5-103">Probleme la ștergerea elementelor SharePoint?</span><span class="sxs-lookup"><span data-stu-id="76de5-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="76de5-104">Asigurați-vă întotdeauna că aveți [permisiunile corespunzătoare](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) pentru a șterge elementul sau aveți un [administrator de colecție de site-ul](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) încearcă să eliminați elementul.</span><span class="sxs-lookup"><span data-stu-id="76de5-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="76de5-105">Asigurați-vă că nu există o setare de [politică de retenție](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pe element.</span><span class="sxs-lookup"><span data-stu-id="76de5-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="76de5-106">Asigurați-vă că elementul nu este [verificat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) la un alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="76de5-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="76de5-107">În cele din urmă, administratorii pot utiliza [modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni complexe de gestionare, ar fi forța ștergerea elemente încăpățânate.</span><span class="sxs-lookup"><span data-stu-id="76de5-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="76de5-108">Eliminare fișier PNP</span><span class="sxs-lookup"><span data-stu-id="76de5-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="76de5-109">Eliminare folder PNP</span><span class="sxs-lookup"><span data-stu-id="76de5-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="76de5-110">Eliminare element listă PNP</span><span class="sxs-lookup"><span data-stu-id="76de5-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="76de5-111">Eliminare listă PNP</span><span class="sxs-lookup"><span data-stu-id="76de5-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="76de5-112">Eliminare câmp PNP (coloană)</span><span class="sxs-lookup"><span data-stu-id="76de5-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)