---
title: Citirea jurnalelor de audit pentru evenimentele șterse
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483315"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="c5a95-102">Citirea jurnalelor de audit pentru evenimentele șterse</span><span class="sxs-lookup"><span data-stu-id="c5a95-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="c5a95-103">Iată cum să procedați:</span><span class="sxs-lookup"><span data-stu-id="c5a95-103">Here's how to do this:</span></span>

1. <span data-ttu-id="c5a95-104">Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="c5a95-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="c5a95-105">Selectați căutare în  >  [**Jurnalul de auditare**](https://go.microsoft.com/fwlink/?linkid=2103759)căutare.</span><span class="sxs-lookup"><span data-stu-id="c5a95-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="c5a95-106">Dacă vedeți o notificare că trebuie să activați caracteristica, mergeți mai departe și activați-o acum.</span><span class="sxs-lookup"><span data-stu-id="c5a95-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="c5a95-107">Dacă caracteristica nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.</span><span class="sxs-lookup"><span data-stu-id="c5a95-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="c5a95-108">Selectați **activități**, apoi găsiți **activități de cutie poștală Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c5a95-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="c5a95-109">Selectați **mesajele șterse din folderul Elemente șterse** și **mutați mesajele în Opțiuni folder Elemente șterse** .</span><span class="sxs-lookup"><span data-stu-id="c5a95-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="c5a95-110">Când ați terminat, faceți clic în exteriorul panoului pentru a minimiza panoul **activități** .</span><span class="sxs-lookup"><span data-stu-id="c5a95-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="c5a95-111">Specificați intervalul de date, apoi, în caseta **utilizatori** , selectați numele de utilizator al utilizatorului pe care doriți să-l anchetați.</span><span class="sxs-lookup"><span data-stu-id="c5a95-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="c5a95-112">Puteți selecta mai mulți utilizatori în același timp.</span><span class="sxs-lookup"><span data-stu-id="c5a95-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="c5a95-113">Selectați **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="c5a95-113">Select **Search**.</span></span> <span data-ttu-id="c5a95-114">Activitățile apar sub **Rezultate**.</span><span class="sxs-lookup"><span data-stu-id="c5a95-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="c5a95-115">Pentru a vizualiza detaliile, selectați o activitate, apoi selectați **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="c5a95-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="c5a95-116">Informații suplimentare despre elementul șters, cum ar fi linia de subiect și locația elementului atunci când a fost șters, se afișează în câmpul **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="c5a95-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="c5a95-117">Nu puteți restaura elementele șterse utilizând caracteristica jurnal de auditare.</span><span class="sxs-lookup"><span data-stu-id="c5a95-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="c5a95-118">Pentru a restaura elementele șterse, consultați [Recuperarea elementelor șterse sau a e-mailului în Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="c5a95-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="c5a95-119">Pentru a afla mai multe, consultați [Căutați în Jurnalul de audit Office 365 pentru a depana scenarii comune](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="c5a95-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
