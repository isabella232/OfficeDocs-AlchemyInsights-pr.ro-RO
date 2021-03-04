---
title: Găsirea evenimentelor efectuate în regulile de Inbox
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430014"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="ab07a-102">Găsirea evenimentelor efectuate în regulile de Inbox</span><span class="sxs-lookup"><span data-stu-id="ab07a-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="ab07a-103">Atunci când sunt create, modificate sau șterse reguli pentru Inbox, evenimentele sunt înregistrate în Jurnalul de auditare.</span><span class="sxs-lookup"><span data-stu-id="ab07a-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="ab07a-104">Iată cum să le revizuiți:</span><span class="sxs-lookup"><span data-stu-id="ab07a-104">Here's how to review them:</span></span>

1. <span data-ttu-id="ab07a-105">Accesați centrul de [conformitate & securitate Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ab07a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ab07a-106">Selectați Căutare > căutare în Jurnalul de auditare.</span><span class="sxs-lookup"><span data-stu-id="ab07a-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ab07a-107">Dacă vedeți o notificare că trebuie să activați auditarea, mergeți mai departe și activați-o acum.</span><span class="sxs-lookup"><span data-stu-id="ab07a-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ab07a-108">Dacă această caracteristică nu este activată, rezultatele căutării nu vor putea să tragă date din datele anterioare.</span><span class="sxs-lookup"><span data-stu-id="ab07a-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ab07a-109">Selectați câmpul activități și găsiți activități de cutie poștală Exchange, apoi selectați New-InboxRule creați o regulă de Inbox din Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ab07a-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="ab07a-110">Când ați terminat, faceți clic în exteriorul panoului pentru a minimiza panoul activități.</span><span class="sxs-lookup"><span data-stu-id="ab07a-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="ab07a-111">Specificați intervalul de date, apoi, în câmpul utilizatori, selectați numele de utilizator al utilizatorului pe care doriți să-l anchetați.</span><span class="sxs-lookup"><span data-stu-id="ab07a-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="ab07a-112">Puteți selecta mai mulți utilizatori în același timp.</span><span class="sxs-lookup"><span data-stu-id="ab07a-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="ab07a-113">Selectați căutare.</span><span class="sxs-lookup"><span data-stu-id="ab07a-113">Select Search.</span></span> <span data-ttu-id="ab07a-114">Activitățile apar sub rezultate.</span><span class="sxs-lookup"><span data-stu-id="ab07a-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="ab07a-115">Pentru a vizualiza detaliile, selectați o activitate, apoi selectați mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="ab07a-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="ab07a-116">Sub secțiunea parametri, puteți vedea numele regulii, setul de condiții și acțiunile pe care le va lua regula.</span><span class="sxs-lookup"><span data-stu-id="ab07a-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="ab07a-117">Pentru a afla mai multe, consultați căutați în Jurnalul de audit Office 365 pentru a depana scenarii comune.</span><span class="sxs-lookup"><span data-stu-id="ab07a-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>