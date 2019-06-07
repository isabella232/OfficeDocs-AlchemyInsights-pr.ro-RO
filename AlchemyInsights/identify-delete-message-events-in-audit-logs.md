---
title: Identifica Ştergere mesaj evenimente în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755164"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="04c62-102">Jurnalele de auditare pentru mesaje e-mail şterse</span><span class="sxs-lookup"><span data-stu-id="04c62-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="04c62-103">Începând din ianuarie 2019, Microsoft este de cotitură pe cutie poştală de audit logare în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="04c62-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="04c62-104">În caz contrar, pentru a revizui Ştergere mesaj evenimente pentru un anumit utilizator, trebuie să activaţi manual delete acţiunile de auditare.</span><span class="sxs-lookup"><span data-stu-id="04c62-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="04c62-105">În cazul în care cutia poştală de audit logare deja este activată pentru organizaţie sau de utilizator specifice, urmaţi paşii de mai jos.</span><span class="sxs-lookup"><span data-stu-id="04c62-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="04c62-106">Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="04c62-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="04c62-107">Faceţi clic pe **Căutare şi ancheta** şi selectaţi **Căutare de jurnalul de Audit**.</span><span class="sxs-lookup"><span data-stu-id="04c62-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="04c62-108">Selectaţi intervalul de date în câmpurile **data de început** şi **data de sfârşit** .</span><span class="sxs-lookup"><span data-stu-id="04c62-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="04c62-109">Specificaţi numele de utilizator pentru utilizator pe care doriţi să investigheze (utilizatorul care elemente şterse).</span><span class="sxs-lookup"><span data-stu-id="04c62-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="04c62-110">În câmpul de **activităţi** , selectaţi **mesajele şterse din folderul Elemente şterse** şi **mesaje de mutat în folderul Elemente şterse**.</span><span class="sxs-lookup"><span data-stu-id="04c62-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="04c62-111">Faceţi clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="04c62-111">Click **Search**.</span></span>

<span data-ttu-id="04c62-112">În rezultate, selectaţi o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="04c62-112">In the results, select an audit record.</span></span> <span data-ttu-id="04c62-113">În fișă de detalii, faceţi clic pe **Mai multe informaţii**.</span><span class="sxs-lookup"><span data-stu-id="04c62-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="04c62-114">Informaţii suplimentare despre element şters (de exemplu, subiectul şi locaţia elementului atunci când a fost sters) este afişat în câmpul **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="04c62-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="04c62-115">Proprietatea **ClientInfoString** va arăta dacă ştergerea a avut loc în Outlook, Outlook web (cunoscut anterior ca Outlook Web App), sau orice alt dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="04c62-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="04c62-116">Pentru informaţii suplimentare, consultaţi [determină care configurarea e-mail forwarding pentru o cutie poştală](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="04c62-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="04c62-117">**Notă**: Imposibil de regăsit elementele şterse utilizând caracteristica de jurnalul de audit.</span><span class="sxs-lookup"><span data-stu-id="04c62-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="04c62-118">Pentru a prelua mesajele şterse în Outlook pe web, a se vedea [a nota a şterge elemente din Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="04c62-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
