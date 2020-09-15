---
title: Identificarea redirecționarii e-mailurilor externe în cutiile poștale din jurnalele de audit
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696309"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="1f238-102">Identificarea când se configurează redirecționarea e-mailurilor externe în cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="1f238-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="1f238-103">Atunci când un utilizator Microsoft 365 configurează redirecționarea e-mailurilor externe într-o cutie poștală, activitatea este auditată ca parte din cmdletul **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="1f238-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="1f238-104">Puteți vedea activitatea utilizând căutarea în Jurnalul de audit din centrul de conformitate & de securitate.</span><span class="sxs-lookup"><span data-stu-id="1f238-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="1f238-105">Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1f238-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1f238-106">Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.</span><span class="sxs-lookup"><span data-stu-id="1f238-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="1f238-107">Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** .</span><span class="sxs-lookup"><span data-stu-id="1f238-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="1f238-108">Nu trebuie să specificați un nume de utilizator.</span><span class="sxs-lookup"><span data-stu-id="1f238-108">You don't need to specify a username.</span></span> <span data-ttu-id="1f238-109">Verificați dacă câmpul **activități** este setat să **afișeze rezultate pentru toate activitățile**.</span><span class="sxs-lookup"><span data-stu-id="1f238-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="1f238-110">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="1f238-110">Click **Search**.</span></span>

<span data-ttu-id="1f238-111">În rezultate, faceți clic pe **Filtrare rezultate** și tastați **set-cutie poștală** în caseta Filtru activitate.</span><span class="sxs-lookup"><span data-stu-id="1f238-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="1f238-112">Selectați o înregistrare de auditare în rezultate.</span><span class="sxs-lookup"><span data-stu-id="1f238-112">Select an audit record in the results.</span></span> <span data-ttu-id="1f238-113">În flyout **Detalii** , faceți clic pe **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="1f238-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="1f238-114">Trebuie să examinați detaliile fiecărei înregistrări de audit pentru a determina dacă activitatea este corelată cu redirecționarea e-mailului.</span><span class="sxs-lookup"><span data-stu-id="1f238-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="1f238-115">**ObjectID**: valoarea alias a cutiei poștale care a fost modificată.</span><span class="sxs-lookup"><span data-stu-id="1f238-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="1f238-116">**Parametri**: _ForwardingSmtpAddress_ indică adresa de e-mail țintă.</span><span class="sxs-lookup"><span data-stu-id="1f238-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="1f238-117">**ID**utilizator: utilizatorul care a configurat redirecționarea mesajelor de e-mail în cutia poștală din câmpul **objectID** .</span><span class="sxs-lookup"><span data-stu-id="1f238-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="1f238-118">Pentru mai multe informații, consultați [cum se determină cine configurează redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="1f238-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
