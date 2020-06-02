---
title: Identificarea redirecționării externe a e-mailurilor în cutiile poștale în jurnalele de audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508964"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="e1493-102">Identificarea când este configurată redirecționarea e-mailurilor externe în cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="e1493-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="e1493-103">Atunci când un utilizator Microsoft 365 configurează redirecționarea de e-mail extern pe o cutie poștală, activitatea este auditat ca parte a cmdletului **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e1493-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="e1493-104">Puteți vedea activitatea utilizând căutarea jurnalului de audit în Centrul de securitate & conformitate.</span><span class="sxs-lookup"><span data-stu-id="e1493-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="e1493-105">Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e1493-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e1493-106">Accesați pagina **Search**  >  **de căutare în jurnalul De audit căutare.**</span><span class="sxs-lookup"><span data-stu-id="e1493-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e1493-107">Selectați intervalul de date din câmpurile **Data de început** și data de **sfârșit.**</span><span class="sxs-lookup"><span data-stu-id="e1493-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e1493-108">Nu este necesar să specificați un nume de utilizator.</span><span class="sxs-lookup"><span data-stu-id="e1493-108">You don't need to specify a username.</span></span> <span data-ttu-id="e1493-109">Verificați că câmpul **Activități** este setat la **Afișare rezultate pentru toate activitățile**.</span><span class="sxs-lookup"><span data-stu-id="e1493-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="e1493-110">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="e1493-110">Click **Search**.</span></span>

<span data-ttu-id="e1493-111">În rezultate, faceți clic pe **Filtrare rezultate** și tastați **Set-Mailbox** în caseta filtru activitate.</span><span class="sxs-lookup"><span data-stu-id="e1493-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="e1493-112">Selectați o înregistrare de audit în rezultate.</span><span class="sxs-lookup"><span data-stu-id="e1493-112">Select an audit record in the results.</span></span> <span data-ttu-id="e1493-113">În flyout **detalii,** faceți clic pe **Mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="e1493-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="e1493-114">Trebuie să analizați detaliile fiecărei înregistrări de audit pentru a determina dacă activitatea este legată de redirecționarea e-mailurilor.</span><span class="sxs-lookup"><span data-stu-id="e1493-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="e1493-115">**ObjectId**: Valoarea alias a cutiei poștale care a fost modificată.</span><span class="sxs-lookup"><span data-stu-id="e1493-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="e1493-116">**Parametri:** _RedirecționareSmtpAddress_ indică adresa de e-mail țintă.</span><span class="sxs-lookup"><span data-stu-id="e1493-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="e1493-117">**UserId**: Utilizatorul care a configurat redirecționarea e-mail ului pe cutia poștală în câmpul **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="e1493-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="e1493-118">Pentru mai multe informații, consultați [Determinarea cine a configurat redirecționarea e-mailului pentru o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e1493-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
