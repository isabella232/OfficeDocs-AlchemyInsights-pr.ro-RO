---
title: Identificarea activității de regulă inbox în jurnalele de audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716436"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ed90c-102">Identificarea activității de regulă inbox în jurnalele de audit</span><span class="sxs-lookup"><span data-stu-id="ed90c-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ed90c-103">Aveți posibilitatea să utilizați căutarea în jurnal de audit în Centrul de conformitate Microsoft 365 security & pentru a vizualiza evenimentele de regulă din inbox (crearea, modificarea și ștergerea regulilor inbox).</span><span class="sxs-lookup"><span data-stu-id="ed90c-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ed90c-104">Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ed90c-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ed90c-105">Accesați pagina de căutare în jurnalul **De** > **audit căutare.**</span><span class="sxs-lookup"><span data-stu-id="ed90c-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ed90c-106">Selectați intervalul de date din câmpurile **Data de început** și data de **sfârșit.**</span><span class="sxs-lookup"><span data-stu-id="ed90c-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ed90c-107">Sub **Activități cutie poștală Exchange**, verificați câmpul **activități** este setată la **New-InboxRule Create/modify/enable/disable inbox regulă**.</span><span class="sxs-lookup"><span data-stu-id="ed90c-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ed90c-108">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="ed90c-108">Click **Search**.</span></span>

<span data-ttu-id="ed90c-109">În rezultate, selectați o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="ed90c-109">In the results, select an audit record.</span></span> <span data-ttu-id="ed90c-110">În detalii flyout, faceți clic pe **Mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="ed90c-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ed90c-111">Informațiidespre setările regulii inbox se afișează în câmpul **Parametri.**</span><span class="sxs-lookup"><span data-stu-id="ed90c-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ed90c-112">Pentru mai multe informații, consultați [Determinarea dacă un utilizator a creat o regulă inbox](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="ed90c-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
