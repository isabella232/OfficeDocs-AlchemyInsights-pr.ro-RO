---
title: Identifica externe e-mail forwarding pe cutiile poştale în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752031"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="d9466-102">Identifica atunci când extern e-mail forwarding este configurat pe cutiile poştale</span><span class="sxs-lookup"><span data-stu-id="d9466-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="d9466-103">Atunci când un utilizator se configurează externe e-mail forwarding pe o cutie poştală, activitatea este auditate ca parte a cmdlet-ul **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="d9466-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="d9466-104">Puteţi vedea activitatea folosind audit jurnal caută în & de securitate centru de conformitate.</span><span class="sxs-lookup"><span data-stu-id="d9466-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="d9466-105">Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d9466-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d9466-106">Faceţi clic pe **Căutare şi ancheta** şi selectaţi **Căutare de jurnalul de Audit**.</span><span class="sxs-lookup"><span data-stu-id="d9466-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d9466-107">Selectaţi intervalul de date în câmpurile **data de început** şi **data de sfârşit** .</span><span class="sxs-lookup"><span data-stu-id="d9466-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d9466-108">Nu aveţi nevoie să specificaţi un nume de utilizator.</span><span class="sxs-lookup"><span data-stu-id="d9466-108">You don't need to specify a username.</span></span> <span data-ttu-id="d9466-109">Verificaţi câmpul de **activităţi** este setată pentru a **afişa rezultate pentru toate acțiunile**.</span><span class="sxs-lookup"><span data-stu-id="d9466-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="d9466-110">Faceţi clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="d9466-110">Click **Search**.</span></span>

<span data-ttu-id="d9466-111">În rezultate, faceţi clic pe **Filtru rezultate** şi **Set-Mailbox** de tip în caseta filtru de activitate.</span><span class="sxs-lookup"><span data-stu-id="d9466-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="d9466-112">Selectaţi o înregistrare de audit în rezultate.</span><span class="sxs-lookup"><span data-stu-id="d9466-112">Select an audit record in the results.</span></span> <span data-ttu-id="d9466-113">În fișă de **Detalii** , faceţi clic pe **mai multe informaţii**.</span><span class="sxs-lookup"><span data-stu-id="d9466-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="d9466-114">Trebuie sa te uiti la detalii cu privire la fiecare înregistrare de audit pentru a determina dacă activitatea este legată de e-mail forwarding.</span><span class="sxs-lookup"><span data-stu-id="d9466-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="d9466-115">**ObjectId**: valoarea aliasul cutiei poştale care s-a modificat.</span><span class="sxs-lookup"><span data-stu-id="d9466-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="d9466-116">**Parametrii**: _ForwardingSmtpAddress_ indică adresa de email ţintă.</span><span class="sxs-lookup"><span data-stu-id="d9466-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="d9466-117">**ID utilizator**: utilizatorului care a configurat expediere poştă electronică din cutia poştală în domeniul **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="d9466-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="d9466-118">Pentru informaţii suplimentare, consultaţi [determină care configurarea e-mail forwarding pentru o cutie poştală](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d9466-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
