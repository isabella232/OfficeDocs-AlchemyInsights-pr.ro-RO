---
title: Rapoarte de jurnal de audit Are A fi audiate SharePoint clasice
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741977"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ae56e-102">Jurnalele de audit SharePoint și OneDrive</span><span class="sxs-lookup"><span data-stu-id="ae56e-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ae56e-103">Jurnalele de audit clasic SharePoint</span><span class="sxs-lookup"><span data-stu-id="ae56e-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ae56e-104">Auditul moștenit spo a fost migrat în Jurnalul de audit unificat (UAL).</span><span class="sxs-lookup"><span data-stu-id="ae56e-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ae56e-105">Toate rapoartele de audit moștenite SPO vor fi alimentate acum prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.</span><span class="sxs-lookup"><span data-stu-id="ae56e-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ae56e-106">Modificări cheie:</span><span class="sxs-lookup"><span data-stu-id="ae56e-106">Key changes:</span></span>

* <span data-ttu-id="ae56e-107">Tunderea NU este disponibilă ca o capacitate.</span><span class="sxs-lookup"><span data-stu-id="ae56e-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ae56e-108">Alegerea evenimentelor specifice pentru audit NU este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="ae56e-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ae56e-109">Consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="ae56e-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ae56e-110">Opțiunea **Locație** sub **Rapoarte personalizate** NU este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="ae56e-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ae56e-111">Opțiunea **Deschiderea sau descărcarea evenimentelor de documente** NU este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="ae56e-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ae56e-112">Configurarea setărilor de audit pentru o colecție de site-uri</span><span class="sxs-lookup"><span data-stu-id="ae56e-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ae56e-113">Jurnalele de audit unificat emititație SharePoint și OneDrive Modern Unified Audit din conformitate</span><span class="sxs-lookup"><span data-stu-id="ae56e-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ae56e-114">Activarea/dezactivarea înregistrării în jurnal unificate a auditului</span><span class="sxs-lookup"><span data-stu-id="ae56e-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ae56e-115">Nu este necesară o configurație suplimentară în SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ae56e-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ae56e-116">Utilizați căutarea în jurnal de auditare pentru a verifica activitatea fișierelor, folderelor, utilizatorului (utilizatorilor), permisiunilor:</span><span class="sxs-lookup"><span data-stu-id="ae56e-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ae56e-117">Activități de fișiere și pagini</span><span class="sxs-lookup"><span data-stu-id="ae56e-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ae56e-118">Activități de foldere</span><span class="sxs-lookup"><span data-stu-id="ae56e-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ae56e-119">Partajarea și activitățile de solicitare a accesului</span><span class="sxs-lookup"><span data-stu-id="ae56e-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ae56e-120">Activități de sincronizare</span><span class="sxs-lookup"><span data-stu-id="ae56e-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ae56e-121">Activități de administrare a sitului</span><span class="sxs-lookup"><span data-stu-id="ae56e-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ae56e-122">Pentru mai multe informații despre să regăsiți aceste evenimente, consultați [Căutarea în jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ae56e-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
