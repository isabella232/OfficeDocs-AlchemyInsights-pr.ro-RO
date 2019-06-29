---
title: 1336 RecoverableItems dosarul este complet
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370399"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="56750-102">Folderul Elemente recuperabile este plin</span><span class="sxs-lookup"><span data-stu-id="56750-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="56750-103">Pentru poştale Exchange Online în Office 365, limita de stocare implicită pentru folderul Elemente recuperabile este 30 GB.</span><span class="sxs-lookup"><span data-stu-id="56750-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="56750-104">Limita de stocare pentru folderul Elemente recuperabile este crescut automat la 100 GB, în cazul în care cutia poştală este plasat litigii Hold, ţineţi eDiscovery, sau este asociată o politică de retenție Office 365.</span><span class="sxs-lookup"><span data-stu-id="56750-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="56750-105">Când folderul Elemente recuperabile atinge limita de stocare, funcţionalitatea de cutie poştală este afectată în următoarele moduri:</span><span class="sxs-lookup"><span data-stu-id="56750-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="56750-106">Utilizatorul nu poate şterge elemente din cutia poştală.</span><span class="sxs-lookup"><span data-stu-id="56750-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="56750-107">Asistentul pentru foldere gestionate nu se poate şterge elemente bazate pe etichetă de conservare sau setările de foldere gestionate.</span><span class="sxs-lookup"><span data-stu-id="56750-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="56750-108">Pentru cutiile poştale care au singur element recuperare permis sau sunt puse pe "hold", procesul de protecţie copia pe scrie filme nu poate menține versiuni de articole editate de catre utilizator.</span><span class="sxs-lookup"><span data-stu-id="56750-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="56750-109">Pentru cutiile poştale care au cutii poştale activate de logare de audit, nici o cutie poştală de audit intrări jurnal pot fi salvate în subfolderul de audit din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="56750-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="56750-110">Pentru cutiile poştale care nu sunt pe "hold", puteţi utiliza administratori `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comanda în Exchange Online PowerShell să ştergeţi elementele din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="56750-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="56750-111">Pentru informații suplimentare, consultați următoarele articole:</span><span class="sxs-lookup"><span data-stu-id="56750-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="56750-112">Căuta şi a şterge mesaje</span><span class="sxs-lookup"><span data-stu-id="56750-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="56750-113">Cutia poştală de căutare</span><span class="sxs-lookup"><span data-stu-id="56750-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="56750-114">Pentru cutiile poştale care sunt pe "hold", administratorii trebuie să eliminaţi Cala înainte ei a putea elementele şterse din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="56750-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="56750-115">Pentru informaţii suplimentare, consultaţi [ştergeţi elementele din Elemente recuperabile folderul de cutii poştale din cadrul norului pe hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="56750-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="56750-116">Pentru a preveni folderul Elemente recuperabile de a deveni complet, administratorii pot creşte limita de stocare de Elemente recuperabile pliant pentru cutiile poştale pe hold şi a înfiinţat o cutie poştală conservare care mută elementele din folderul Elemente recuperabile al utilizatorului Arhiva cutie poştală.</span><span class="sxs-lookup"><span data-stu-id="56750-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="56750-117">Consultaţi [creşte Elemente recuperabile cotelor pentru cutii poştale pe hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="56750-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
