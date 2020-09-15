---
title: Rapoarte jurnal de audit SharePoint clasic
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662220"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="a9e62-102">Jurnalele de audit SharePoint și OneDrive</span><span class="sxs-lookup"><span data-stu-id="a9e62-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="a9e62-103">Jurnalele de audit SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="a9e62-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="a9e62-104">Auditarea moștenită SPO a fost migrată în jurnal de audit unificat (nepotrivit).</span><span class="sxs-lookup"><span data-stu-id="a9e62-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="a9e62-105">Toate rapoartele de audit moștenite de la SPO vor fi alimentate acum prin intermediul, iar semnalele de audit moștenite au fost migrate la un raport.</span><span class="sxs-lookup"><span data-stu-id="a9e62-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="a9e62-106">Modificări cheie:</span><span class="sxs-lookup"><span data-stu-id="a9e62-106">Key changes:</span></span>

* <span data-ttu-id="a9e62-107">Tunderea nu este disponibilă ca o capacitate.</span><span class="sxs-lookup"><span data-stu-id="a9e62-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="a9e62-108">Nu este disponibilă alegerea anumitor evenimente de auditare.</span><span class="sxs-lookup"><span data-stu-id="a9e62-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="a9e62-109">Consultați [acest document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="a9e62-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="a9e62-110">Opțiunea **locație** de sub **rapoarte particularizate** nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="a9e62-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="a9e62-111">Opțiunea **Deschidere sau descărcare documente** evenimente nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="a9e62-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="a9e62-112">Configurarea setărilor de audit pentru o colecție de site-uri</span><span class="sxs-lookup"><span data-stu-id="a9e62-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="a9e62-113">Jurnalele de audit unificate moderne SharePoint și OneDrive de la conformitate</span><span class="sxs-lookup"><span data-stu-id="a9e62-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="a9e62-114">Activarea/dezactivarea înregistrării în jurnal a auditării unificate</span><span class="sxs-lookup"><span data-stu-id="a9e62-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="a9e62-115">Nu este necesară nicio configurare suplimentară în SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a9e62-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="a9e62-116">Utilizarea căutării în înregistrarea în jurnal a auditării pentru a verifica activitatea fișierelor, a folderelor, a utilizatorilor, a permisiunilor:</span><span class="sxs-lookup"><span data-stu-id="a9e62-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="a9e62-117">Activități de fișier și de pagină</span><span class="sxs-lookup"><span data-stu-id="a9e62-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="a9e62-118">Activități de foldere</span><span class="sxs-lookup"><span data-stu-id="a9e62-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="a9e62-119">Activități de partajare și de solicitare a accesului</span><span class="sxs-lookup"><span data-stu-id="a9e62-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="a9e62-120">Activități de sincronizare</span><span class="sxs-lookup"><span data-stu-id="a9e62-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="a9e62-121">Activități de administrare a site-ului</span><span class="sxs-lookup"><span data-stu-id="a9e62-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="a9e62-122">Pentru mai multe informații despre cum să regăsiți aceste evenimente, consultați [căutarea în Jurnalul de auditare](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="a9e62-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
