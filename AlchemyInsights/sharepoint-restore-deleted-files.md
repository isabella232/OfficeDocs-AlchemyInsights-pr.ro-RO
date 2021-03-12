---
title: Restaurarea unui fișier sau folder șters
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707534"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="9c6d5-102">Restaurarea unui fișier sau folder șters</span><span class="sxs-lookup"><span data-stu-id="9c6d5-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="9c6d5-103">SharePoint Online păstrează copiile de rezervă ale întregului conținut timp de 14 zile suplimentare în afara ștergerii efective.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="9c6d5-104">Dacă conținutul nu poate fi restaurat prin Coșul de reciclare sau restaurarea fișierelor, un administrator poate contacta asistența Microsoft pentru a solicita o restaurare în orice moment din fereastra de 14 zile.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="9c6d5-105">Restaurarea din copiile de backup poate fi finalizată doar pentru colecțiile de site-uri sau pentru subsite-urile, nu pentru anumite fișiere, liste sau biblioteci.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="9c6d5-106">Atunci când ștergeți un element sau un site din SharePoint, acesta nu este eliminat imediat.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="9c6d5-107">Elementele șterse intră în coșul de reciclare pentru un interval de timp.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="9c6d5-108">În acest timp, puteți restaura elementele pe care le-ați șters în locația lor originală.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="9c6d5-109">Pentru mai multe informații, vizitați linkurile de mai jos.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="9c6d5-110">[Restaurarea elementelor din Coșul de reciclare al unui site SharePoint](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span><span class="sxs-lookup"><span data-stu-id="9c6d5-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="9c6d5-111">Restaurarea fișierelor sau folderelor șterse în OneDrive</span><span class="sxs-lookup"><span data-stu-id="9c6d5-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="9c6d5-112">Restaurarea unei colecții de site-uri șterse (inclusiv grup, comunicare și alte site-uri)</span><span class="sxs-lookup"><span data-stu-id="9c6d5-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="9c6d5-113">Restaurarea unui site OneDrive șters</span><span class="sxs-lookup"><span data-stu-id="9c6d5-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="9c6d5-114">Pentru acțiunile din Coșul de reciclare masiv, administratorii pot lua în considerare utilizarea [SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="9c6d5-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="9c6d5-115">**Caracteristica Restaurare fișiere**</span><span class="sxs-lookup"><span data-stu-id="9c6d5-115">**Files Restore feature**</span></span>

<span data-ttu-id="9c6d5-116">Dacă o mulțime de fișiere OneDrive sau SharePoint sunt șterse, suprascrise, deteriorate sau infectate prin malware, puteți să restaurați întreaga bibliotecă OneDrive sau SharePoint la o oră anterioară, utilizând caracteristica Restaurare fișiere.</span><span class="sxs-lookup"><span data-stu-id="9c6d5-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="9c6d5-117">Restaurarea unei biblioteci OneDrive</span><span class="sxs-lookup"><span data-stu-id="9c6d5-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="9c6d5-118">Restaurarea unei biblioteci de documente</span><span class="sxs-lookup"><span data-stu-id="9c6d5-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

