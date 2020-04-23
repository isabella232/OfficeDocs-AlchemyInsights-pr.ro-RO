---
title: Notificări de alertă SharePoint nu sunt livrate
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742059"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="6a9f6-102">Notificări de alertă SharePoint nu sunt livrate</span><span class="sxs-lookup"><span data-stu-id="6a9f6-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="6a9f6-103">Verificați folderul JUNK din e-mail, deoarece uneori alertele ar putea merge acolo.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="6a9f6-104">Determinați dacă **toate avertizările nu sunt livrate** sau dacă nu este **livrată o avertizare individuală** dintr-un anumit fișier sau bibliotecă.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="6a9f6-105">**Alerte individuale nu sunt livrate:** Dacă o avertizare individuală dintr-un anumit fișier sau bibliotecă nu este livrată, puteți încerca să o ștergeți și să o creați din nou.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="6a9f6-106">Consultați [Gestionarea, vizualizarea sau ștergerea alertelor SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) pentru a recrea alerta.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="6a9f6-107">**Toate alertele nu sunt livrate:** Dacă nu sunt livrate toate alertele din mai multe fișiere sau biblioteci, vizitați [tabloul de bord Sănătate serviciu](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a verifica orice recomandări/incidente care pot apărea cu SharePoint sau Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="6a9f6-108">Problema ar putea fi cu capacitatea de alertă SharePoint sau întârzieri în e-mailuri prin Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="6a9f6-109">De asemenea, va fi important să rețineți dacă alte e-mail este livrat, și dacă nu, problema este probabil cu întârzieri Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="6a9f6-110">Întrebări frecvente despre alerte:</span><span class="sxs-lookup"><span data-stu-id="6a9f6-110">FAQ on alerts:</span></span>

- <span data-ttu-id="6a9f6-111">Nu este posibil să trimiteți alerte grupului de distribuire, sunt acceptate numai grupurile Security și O365.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="6a9f6-112">Nu aveți posibilitatea să particularizați șabloanele de e-mail de avertizare; trebuie să utilizați Fluxul de lucru Microsoft FLOW sau SharePoint Designer pentru a le atinge.</span><span class="sxs-lookup"><span data-stu-id="6a9f6-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="6a9f6-113">Mai multe informații:</span><span class="sxs-lookup"><span data-stu-id="6a9f6-113">More Information:</span></span>

- <span data-ttu-id="6a9f6-114">**Configurare a alertei**: Pentru mai multe informații despre configurarea avertizărilor, consultați [Crearea unei alerte pentru a fi notificată atunci când un fișier sau un folder se modifică în SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="6a9f6-115">**Depanarea avertizărilor**: Pentru mai multe informații despre depanarea avertizărilor, consultați [Utilizatorii nu primesc notificări de avertizare SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="6a9f6-116">**Politici avansate de alertă de conformitate O365:** Pentru mai multe informații despre configurarea acestor alerte, consultați [Politicile de alertă de conformitate](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="6a9f6-117">**Jurnalele de audit SharePoint și OneDrive:** Pentru mai multe informații despre să regăsiți aceste evenimente, consultați [Căutarea jurnalului de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="6a9f6-118">**Alerte trimise de Protecție avansată a amenințărilor:** Consultați [ATP pentru SharePoint și OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="6a9f6-119">**Alerte trimise de poliția de prevenire a pierderilor de date:** Consultați [notificările prin e-mail pentru politicile DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="6a9f6-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6a9f6-120">Subiecte înrudite</span><span class="sxs-lookup"><span data-stu-id="6a9f6-120">Related Topics</span></span>

<span data-ttu-id="6a9f6-121">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6a9f6-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="6a9f6-122">Creare flux</span><span class="sxs-lookup"><span data-stu-id="6a9f6-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="6a9f6-123">SharePoint și Flux</span><span class="sxs-lookup"><span data-stu-id="6a9f6-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
