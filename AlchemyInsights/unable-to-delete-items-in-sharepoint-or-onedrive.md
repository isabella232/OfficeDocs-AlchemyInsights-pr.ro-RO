---
title: Nu se pot șterge elemente în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806123"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="616b6-102">Nu se pot șterge elemente</span><span class="sxs-lookup"><span data-stu-id="616b6-102">Unable to delete items</span></span>

<span data-ttu-id="616b6-103">Politicile de retenție pot provoca acest lucru, trebuie să dezactivați sau să excludeți respectiva fixare care cauzează această problemă.</span><span class="sxs-lookup"><span data-stu-id="616b6-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="616b6-104">După eliminarea unei politici de retenție sau a unei rețineri, poate dura până la 24 de ore pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="616b6-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="616b6-105">Asigurați-vă că nu există o configurare a [politicii de retenție](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pentru element.</span><span class="sxs-lookup"><span data-stu-id="616b6-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="616b6-106">Este posibil ca site-ul să fi depășit limita de stocare, să mărească [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.</span><span class="sxs-lookup"><span data-stu-id="616b6-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="616b6-107">Asigurați-vă că elementul nu este [extras](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) unui alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="616b6-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="616b6-108">În cele din urmă, administratorii pot utiliza [modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni de gestionare complexe, cum ar fi să Impuneți ștergerea elementelor încăpățânat.</span><span class="sxs-lookup"><span data-stu-id="616b6-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="616b6-109">Eliminare fișier PNP</span><span class="sxs-lookup"><span data-stu-id="616b6-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="616b6-110">Eliminare folder PNP</span><span class="sxs-lookup"><span data-stu-id="616b6-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="616b6-111">Eliminare element listă PNP</span><span class="sxs-lookup"><span data-stu-id="616b6-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="616b6-112">Eliminare listă PNP</span><span class="sxs-lookup"><span data-stu-id="616b6-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="616b6-113">Eliminare câmp PNP (coloană)</span><span class="sxs-lookup"><span data-stu-id="616b6-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)