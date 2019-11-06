---
title: Rapoarte de jurnal de audit SharePoint clasic
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992630"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="acaa9-102">Jurnalele de audit SharePoint și OneDrive</span><span class="sxs-lookup"><span data-stu-id="acaa9-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="acaa9-103">Jurnalele de audit clasic SharePoint</span><span class="sxs-lookup"><span data-stu-id="acaa9-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="acaa9-104">Audit moștenire SPO a fost migrat la Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="acaa9-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="acaa9-105">Toate rapoartele de audit moștenite SPO vor fi acum alimentate prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.</span><span class="sxs-lookup"><span data-stu-id="acaa9-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="acaa9-106">Modificări cheie:</span><span class="sxs-lookup"><span data-stu-id="acaa9-106">Key changes:</span></span>

* <span data-ttu-id="acaa9-107">Tundere nu este disponibil ca o capacitate.</span><span class="sxs-lookup"><span data-stu-id="acaa9-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="acaa9-108">Alegerea evenimentelor specifice pentru audit nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="acaa9-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="acaa9-109">Consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="acaa9-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="acaa9-110">Opțiunea de **locație** sub **rapoarte particularizate** nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="acaa9-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="acaa9-111">Opțiunea de **Deschidere sau descărcare documente** de evenimente nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="acaa9-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="acaa9-112">Configurați setările de audit pentru o colecție de site-uri</span><span class="sxs-lookup"><span data-stu-id="acaa9-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="acaa9-113">SharePoint și OneDrive modern audit Unified jurnalele de conformitate</span><span class="sxs-lookup"><span data-stu-id="acaa9-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="acaa9-114">Activați/dezactivați înregistrarea în jurnal a auditului unificat</span><span class="sxs-lookup"><span data-stu-id="acaa9-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="acaa9-115">Nu este necesară nicio configurație suplimentară în SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="acaa9-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="acaa9-116">Utilizați căutarea în jurnal de audit pentru a verifica activitatea fișierului (fișierelor), folderului (ilor), utilizatorilor, permisiunilor:</span><span class="sxs-lookup"><span data-stu-id="acaa9-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="acaa9-117">Activități de fișier și de pagini</span><span class="sxs-lookup"><span data-stu-id="acaa9-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="acaa9-118">Activități folder</span><span class="sxs-lookup"><span data-stu-id="acaa9-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="acaa9-119">Activități de partajare și acces la solicitări</span><span class="sxs-lookup"><span data-stu-id="acaa9-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="acaa9-120">Activități de sincronizare</span><span class="sxs-lookup"><span data-stu-id="acaa9-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="acaa9-121">Activitati de administrare a site-ului</span><span class="sxs-lookup"><span data-stu-id="acaa9-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="acaa9-122">Pentru mai multe informații despre se recuperează aceste evenimente, consultați [Căutați Jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="acaa9-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
