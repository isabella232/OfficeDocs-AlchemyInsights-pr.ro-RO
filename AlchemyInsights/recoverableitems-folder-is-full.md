---
title: folderul RecoverableItems 1336 este plin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741279"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="cd8ff-102">Folderul Elemente recuperabile este plin</span><span class="sxs-lookup"><span data-stu-id="cd8ff-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="cd8ff-103">Pentru cutiile poștale Exchange Online, limita implicită de stocare pentru folderul Elemente recuperabile este 30 GB.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="cd8ff-104">Limita de stocare pentru folderul Elemente recuperabile este mărită automat la 100 GB dacă cutia poștală este plasată în așteptare pentru litigii, descoperire eDiscovery sau este atribuită unei politici de retenție.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="cd8ff-105">Atunci când folderul Elemente recuperabile atinge limita de stocare, funcționalitatea cutiei poștale este afectată în următoarele moduri:</span><span class="sxs-lookup"><span data-stu-id="cd8ff-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="cd8ff-106">Utilizatorul nu poate șterge elemente din cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="cd8ff-107">Asistentul pentru foldere gestionate nu poate șterge elemente pe baza etichetei de retenție sau a setărilor de folder gestionate.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="cd8ff-108">Pentru cutiile poștale care au activată recuperarea unui singur element sau sunt plasate în așteptare, procesul de protecție a paginilor de copiere-la-scriere nu poate menține versiunile de elemente editate de utilizator.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="cd8ff-109">Pentru cutiile poștale care au activată înregistrarea în jurnal a auditării cutiilor poștale, nu se pot salva intrări în jurnal de auditare în caseta de auditare din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="cd8ff-110">Pentru cutiile poștale care nu sunt în așteptare, administratorii pot utiliza `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comanda în Exchange Online PowerShell pentru a șterge elemente din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="cd8ff-111">Pentru informații suplimentare, consultați următoarele articole:</span><span class="sxs-lookup"><span data-stu-id="cd8ff-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="cd8ff-112">Căutarea și ștergerea mesajelor</span><span class="sxs-lookup"><span data-stu-id="cd8ff-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="cd8ff-113">Căutare-cutie poștală</span><span class="sxs-lookup"><span data-stu-id="cd8ff-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="cd8ff-114">Pentru cutiile poștale care sunt în așteptare, administratorii trebuie să elimine suspendarea înainte să poată șterge elemente din folderul Elemente recuperabile.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="cd8ff-115">Pentru mai multe informații, consultați [ștergerea elementelor din folderul Elemente recuperabile din cutiile poștale bazate pe cloud în așteptare](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cd8ff-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="cd8ff-116">Pentru a preveni ca folderul Elemente recuperabile să devină plin, administratorii pot mări limita de stocare a folderului Elemente recuperabile pentru cutiile poștale în așteptare și să configureze o politică de retenție a cutiei poștale care mută elementele din folderul Elemente recuperabile în cutia poștală de arhivă a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="cd8ff-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="cd8ff-117">Consultați [creșterea cotei de Elemente recuperabile pentru cutiile poștale în așteptare](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cd8ff-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
