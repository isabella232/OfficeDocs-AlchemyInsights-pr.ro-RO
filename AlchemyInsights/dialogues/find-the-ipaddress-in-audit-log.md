---
title: Găsirea adresei IP în Jurnalul de auditare
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429788"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="530b6-102">Găsirea adresei IP în Jurnalul de auditare</span><span class="sxs-lookup"><span data-stu-id="530b6-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="530b6-103">Adresa IP care corespunde unei activități efectuate de un utilizator sau administrator este afișată în jurnalele de auditare.</span><span class="sxs-lookup"><span data-stu-id="530b6-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="530b6-104">Informațiile clientului sunt, de asemenea, înregistrate.</span><span class="sxs-lookup"><span data-stu-id="530b6-104">The client information is also logged.</span></span> <span data-ttu-id="530b6-105">Iată cum să identificați adresa IP:</span><span class="sxs-lookup"><span data-stu-id="530b6-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="530b6-106">Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="530b6-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="530b6-107">Selectați căutare în  >  **[Jurnalul de auditare](https://go.microsoft.com/fwlink/?linkid=2103759)** căutare.</span><span class="sxs-lookup"><span data-stu-id="530b6-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="530b6-108">Dacă vedeți o notificare că trebuie să activați auditarea, mergeți mai departe și activați-o acum.</span><span class="sxs-lookup"><span data-stu-id="530b6-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="530b6-109">Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.</span><span class="sxs-lookup"><span data-stu-id="530b6-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="530b6-110">Dacă sunteți interesat de o anumită activitate, selectați-o din lista **activități** ; altfel, în mod implicit, toate activitățile vor fi returnate pentru utilizatorul selectat.</span><span class="sxs-lookup"><span data-stu-id="530b6-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="530b6-111">Rețineți că este posibil ca anumite activități să nu fie disponibile pentru selecție din meniul **activități** ; cu toate acestea, acele elemente de audit vor fi returnate dacă se selectează **Afișare rezultate pentru toate activitățile** (setare implicită).</span><span class="sxs-lookup"><span data-stu-id="530b6-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="530b6-112">Specificați intervalul de date și, în câmpul **utilizatori** , selectați numele de utilizator al utilizatorului pe care doriți să-l anchetați.</span><span class="sxs-lookup"><span data-stu-id="530b6-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="530b6-113">Selectați **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="530b6-113">Select **Search**.</span></span> <span data-ttu-id="530b6-114">Activitățile apar sub **Rezultate**.</span><span class="sxs-lookup"><span data-stu-id="530b6-114">The activities appear under **Results**.</span></span> <span data-ttu-id="530b6-115">Puteți vedea adresa IP pentru fiecare activitate.</span><span class="sxs-lookup"><span data-stu-id="530b6-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="530b6-116">Pentru a vizualiza detaliile, selectați o activitate, apoi selectați **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="530b6-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="530b6-117">Pentru a afla mai multe, consultați căutați în [Jurnalul de audit Office 365 pentru a depana scenarii comune](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="530b6-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>