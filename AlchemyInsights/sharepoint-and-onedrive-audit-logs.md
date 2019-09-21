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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068035"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="fb3e8-102">Jurnalele de audit SharePoint și OneDrive</span><span class="sxs-lookup"><span data-stu-id="fb3e8-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="fb3e8-103">**SharePoint și OneDrive modern audit Unified jurnalele de conformitate**</span><span class="sxs-lookup"><span data-stu-id="fb3e8-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="fb3e8-104">Activați/dezactivați înregistrarea în jurnal a auditului unificat</span><span class="sxs-lookup"><span data-stu-id="fb3e8-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="fb3e8-105">Nu este necesară nicio configurație suplimentară în SharePoint sau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="fb3e8-106">Utilizați căutarea în jurnal de audit pentru a verifica activitatea fișierului (fișierelor), folderului (ilor), utilizatorilor, permisiunilor:</span><span class="sxs-lookup"><span data-stu-id="fb3e8-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="fb3e8-107">Activități de fișier și de pagini</span><span class="sxs-lookup"><span data-stu-id="fb3e8-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="fb3e8-108">Activități folder</span><span class="sxs-lookup"><span data-stu-id="fb3e8-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="fb3e8-109">Activități de partajare și acces la solicitări</span><span class="sxs-lookup"><span data-stu-id="fb3e8-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="fb3e8-110">Activități de sincronizare</span><span class="sxs-lookup"><span data-stu-id="fb3e8-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="fb3e8-111">Activitati de administrare a site-ului</span><span class="sxs-lookup"><span data-stu-id="fb3e8-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="fb3e8-112">Pentru mai multe informații despre se recuperează aceste evenimente, consultați [Căutați Jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="fb3e8-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="fb3e8-113">**Jurnalele de audit clasic SharePoint**</span><span class="sxs-lookup"><span data-stu-id="fb3e8-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="fb3e8-114">Am migrat SPO moștenire de audit pentru Unified audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="fb3e8-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="fb3e8-115">Aceasta înseamnă, în esență, că toate rapoartele de audit moștenite SPO vor fi acum alimentate prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="fb3e8-116">Modificări cheie:</span><span class="sxs-lookup"><span data-stu-id="fb3e8-116">Key changes:</span></span>

- <span data-ttu-id="fb3e8-117">Tundere ca o capacitate nu este disponibil.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="fb3e8-118">Secțiunea în care alegeți evenimente specifice pentru audit nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="fb3e8-119">Vă rugăm să consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod prestabilit.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="fb3e8-120">Opțiunea "locație" sub **rapoarte PARTICULARIZATE** nu este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="fb3e8-121">Evenimentele "deschiderea sau descărcarea documentelor" nu sunt disponibile.</span><span class="sxs-lookup"><span data-stu-id="fb3e8-121">“Opening or downloading documents” events is NOT available.</span></span> 

