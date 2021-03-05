---
title: Aflați cine a configurat redirecționarea la o cutie poștală și cum
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483351"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="05af9-102">Aflați cine a configurat redirecționarea la o cutie poștală și cum</span><span class="sxs-lookup"><span data-stu-id="05af9-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="05af9-103">Dacă redirecționarea externă a fost setată la o cutie poștală, activitatea este auditată ca parte a cmdletului Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="05af9-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="05af9-104">Iată cum să găsiți activitatea în Jurnalul de auditare:</span><span class="sxs-lookup"><span data-stu-id="05af9-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="05af9-105">Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="05af9-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="05af9-106">Selectați căutare în >  **Jurnalul de auditare** căutare.</span><span class="sxs-lookup"><span data-stu-id="05af9-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="05af9-107">Dacă vedeți o notificare că trebuie să activați auditarea, mergeți mai departe și activați-o acum.</span><span class="sxs-lookup"><span data-stu-id="05af9-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="05af9-108">Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.</span><span class="sxs-lookup"><span data-stu-id="05af9-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="05af9-109">Asigurați-vă că câmpul **activități** este setat să **afișeze rezultate pentru toate activitățile** (implicit).</span><span class="sxs-lookup"><span data-stu-id="05af9-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="05af9-110">Specificați intervalul de date.</span><span class="sxs-lookup"><span data-stu-id="05af9-110">Specify the date range.</span></span> <span data-ttu-id="05af9-111">Nu trebuie să specificați un nume de utilizator.</span><span class="sxs-lookup"><span data-stu-id="05af9-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="05af9-112">Selectați **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="05af9-112">Select **Search**.</span></span> <span data-ttu-id="05af9-113">Activitățile apar sub **Rezultate**.</span><span class="sxs-lookup"><span data-stu-id="05af9-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="05af9-114">Selectați **Filtrare rezultate**, apoi introduceți **Set-Mailbox** în câmpul Filtru **activitate** .</span><span class="sxs-lookup"><span data-stu-id="05af9-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="05af9-115">Acest lucru returnează toate activitățile **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="05af9-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="05af9-116">Pentru a vizualiza detaliile, selectați o activitate, apoi selectați **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="05af9-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="05af9-117">Sub **parametri** , puteți vedea adresa de e-mail de redirecționare setată în cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="05af9-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="05af9-118">**ID** -ul de utilizator reprezintă utilizatorul care a configurat redirecționarea externă în cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="05af9-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="05af9-119">Pentru a afla mai multe, consultați [Căutați în Jurnalul de audit Office 365 pentru a depana scenarii comune](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="05af9-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>