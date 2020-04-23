---
title: 1336 RecoverableItems folder este plin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720264"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="816e9-102">Folderul Elemente recuperabile este plin</span><span class="sxs-lookup"><span data-stu-id="816e9-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="816e9-103">Pentru cutiile poștale Exchange Online, limita de stocare implicită pentru folderul Elemente recuperabile este de 30 GO.</span><span class="sxs-lookup"><span data-stu-id="816e9-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="816e9-104">Limita de stocare pentru folderul Elemente recuperabile este mărită automat la 100 GO dacă cutia poștală este plasată în Contencios Hold, eDiscovery hold sau este atribuită unei politici de conservare.</span><span class="sxs-lookup"><span data-stu-id="816e9-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="816e9-105">Când folderul Elemente recuperabile atinge limita de stocare, funcționalitatea cutiei poștale este afectată în următoarele moduri:</span><span class="sxs-lookup"><span data-stu-id="816e9-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="816e9-106">Utilizatorul nu poate șterge elemente din cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="816e9-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="816e9-107">Asistentul folder gestionat nu poate șterge elemente bazate pe eticheta de conservare sau pe setările folderului gestionat.</span><span class="sxs-lookup"><span data-stu-id="816e9-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="816e9-108">Pentru cutiile poștale care au single element de recuperare activat sau sunt plasate în așteptare, procesul de copiere-pe-scrie pagina de protecție nu poate menține versiuni de elemente editate de utilizator.</span><span class="sxs-lookup"><span data-stu-id="816e9-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="816e9-109">Pentru cutiile poștale care au cutie poștală audit înregistrarea în jurnal activat, nu intrările jurnal de audit cutie poștală pot fi salvate în subfolderul audituri în folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="816e9-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="816e9-110">Pentru cutiile poștale care nu sunt în `Search-Mailbox -SearchDumpsterOnly -DeleteContent` așteptare, administratorii pot utiliza comanda în Exchange Online PowerShell pentru a șterge elemente în folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="816e9-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="816e9-111">Pentru informații suplimentare, consultați următoarele articole:</span><span class="sxs-lookup"><span data-stu-id="816e9-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="816e9-112">Căutarea și ștergerea mesajelor</span><span class="sxs-lookup"><span data-stu-id="816e9-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="816e9-113">Caută-Cutie poștală</span><span class="sxs-lookup"><span data-stu-id="816e9-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="816e9-114">Pentru cutiile poștale care sunt în așteptare, administratorii trebuie să eliminați reținerea înainte de a putea șterge elemente din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="816e9-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="816e9-115">Pentru mai multe informații, consultați [Ștergerea elementelor din folderul Elemente recuperabile din cutiile poștale din cadrul norului în așteptare](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="816e9-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="816e9-116">Pentru a preveni folderul Elemente recuperabile de a deveni plin, administratorii pot mări limita de stocare a folderului Elemente recuperabile pentru cutiile poștale în așteptare și configurați o politică de retenție cutie poștală care mută elemente din folderul Elemente recuperabile la cutia poștală de arhivă a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="816e9-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="816e9-117">Consultați [Mărirea cotei elemente recuperabile pentru cutiile poștale în așteptare](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="816e9-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
