---
title: Identificarea evenimentelor de ștergere a mesajelor în jurnalele de auditare
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696525"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="e833a-102">Jurnalele de audit pentru mesajele de e-mail șterse</span><span class="sxs-lookup"><span data-stu-id="e833a-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="e833a-103">Începând din ianuarie 2019, Microsoft pornește înregistrarea în jurnal a auditării cutiilor poștale în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="e833a-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="e833a-104">În caz contrar, pentru a revizui evenimentele de ștergere a mesajelor pentru un anumit utilizator, trebuie să activați manual acțiunile de ștergere pentru auditare.</span><span class="sxs-lookup"><span data-stu-id="e833a-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="e833a-105">Dacă înregistrarea în jurnal a auditării cutiilor poștale este deja activată pentru organizația dumneavoastră sau pentru utilizatorul respectiv, urmați pașii de mai jos.</span><span class="sxs-lookup"><span data-stu-id="e833a-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="e833a-106">Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e833a-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e833a-107">Faceți clic pe **Căutare și investigație** și selectați **Căutare jurnal de auditare**.</span><span class="sxs-lookup"><span data-stu-id="e833a-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e833a-108">Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** .</span><span class="sxs-lookup"><span data-stu-id="e833a-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e833a-109">Specificați numele de utilizator pentru utilizatorul pe care doriți să-l anchetați (utilizatorul care a șters elementele).</span><span class="sxs-lookup"><span data-stu-id="e833a-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="e833a-110">În câmpul **activități** , selectați **mesaje șterse din folderul Elemente șterse** și **mutați mesajele în folderul Elemente șterse**.</span><span class="sxs-lookup"><span data-stu-id="e833a-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="e833a-111">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="e833a-111">Click **Search**.</span></span>

<span data-ttu-id="e833a-112">În rezultate, selectați o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="e833a-112">In the results, select an audit record.</span></span> <span data-ttu-id="e833a-113">În flyout detalii, faceți clic pe **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="e833a-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e833a-114">Informații suplimentare despre elementul șters (de exemplu, linia de subiect și locația elementului atunci când a fost șters) se afișează în câmpul **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="e833a-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="e833a-115">Proprietatea **ClientInfoString** va afișa dacă ștergerea a avut loc în Outlook, Outlook pe web (cunoscut anterior ca Outlook Web App) sau orice alt dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="e833a-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="e833a-116">Pentru mai multe informații, consultați [cum se determină cine configurează redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="e833a-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="e833a-117">**Notă**: nu puteți regăsi elemente șterse utilizând caracteristica jurnal de auditare.</span><span class="sxs-lookup"><span data-stu-id="e833a-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="e833a-118">Pentru a regăsi mesajele șterse în Outlook pe web, consultați [Recuperarea elementelor șterse în Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="e833a-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
