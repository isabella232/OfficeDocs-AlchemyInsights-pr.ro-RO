---
title: Identificarea evenimentelor de ștergere a mesajelor în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716508"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="1f0f7-102">Jurnalele de audit pentru mesajele de e-mail șterse</span><span class="sxs-lookup"><span data-stu-id="1f0f7-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="1f0f7-103">Începând din ianuarie 2019, Microsoft pornește implicit înregistrarea în jurnal a auditului cutiei poștale.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="1f0f7-104">În caz contrar, pentru a examina ștergerea evenimentelor de mesaj pentru un anumit utilizator, trebuie să activați manual acțiunile de ștergere pentru auditare.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="1f0f7-105">Dacă înregistrarea în jurnal a auditului cutiei poștale este deja activată pentru organizația sau pentru utilizatorul specific, urmați pașii de mai jos.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="1f0f7-106">Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1f0f7-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1f0f7-107">Faceți clic pe **Căutare și investigare** și selectați Căutare jurnal **audit**.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1f0f7-108">Selectați intervalul de date din câmpurile **Data de început** și data de **sfârșit.**</span><span class="sxs-lookup"><span data-stu-id="1f0f7-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1f0f7-109">Specificați numele de utilizator pentru utilizatorul pe care doriți să îl investigați (utilizatorul care a șters elementele).</span><span class="sxs-lookup"><span data-stu-id="1f0f7-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="1f0f7-110">În câmpul **Activități,** selectați **Mesaje șterse din folderul Elemente șterse** și **Mesaje mutate în folderul Elemente șterse**.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="1f0f7-111">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-111">Click **Search**.</span></span>

<span data-ttu-id="1f0f7-112">În rezultate, selectați o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-112">In the results, select an audit record.</span></span> <span data-ttu-id="1f0f7-113">În detalii flyout, faceți clic pe **Mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1f0f7-114">Informații suplimentare despre elementul șters (de exemplu, linia de subiect și locația elementului când a fost șters) sunt afișate în câmpul **Elemente afectate.**</span><span class="sxs-lookup"><span data-stu-id="1f0f7-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="1f0f7-115">Proprietatea **ClientInfoString** va afișa dacă ștergerea a avut loc în Outlook, Outlook pe web (cunoscut anterior ca Outlook Web App) sau orice alt dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="1f0f7-116">Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="1f0f7-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="1f0f7-117">**Notă:** Nu puteți regăsi elementele șterse utilizând caracteristica jurnal de auditare.</span><span class="sxs-lookup"><span data-stu-id="1f0f7-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="1f0f7-118">Pentru a prelua mesajele șterse din Outlook pe web, consultați [Recuperarea elementelor șterse în Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="1f0f7-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
