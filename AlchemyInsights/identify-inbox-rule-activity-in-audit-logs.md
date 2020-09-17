---
title: Identificarea activității de regulă Inbox în jurnalele de auditare
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779063"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="a80dc-102">Identificarea activității de regulă Inbox în jurnalele de auditare</span><span class="sxs-lookup"><span data-stu-id="a80dc-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="a80dc-103">Puteți utiliza căutarea în Jurnalul de audit din centrul de conformitate Microsoft 365 Security & pentru a vizualiza evenimentele de regulă pentru Inbox (crearea, modificarea și ștergerea regulilor pentru Inbox).</span><span class="sxs-lookup"><span data-stu-id="a80dc-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="a80dc-104">Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a80dc-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a80dc-105">Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.</span><span class="sxs-lookup"><span data-stu-id="a80dc-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="a80dc-106">Selectați intervalul de date din câmpurile data de **început** și **data de sfârșit** .</span><span class="sxs-lookup"><span data-stu-id="a80dc-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="a80dc-107">Sub **activități de cutie poștală Exchange**, Verificați dacă câmpul **activități** este setat la **nou-InboxRule creare/modificare/Activare/Dezactivare regulă Inbox**.</span><span class="sxs-lookup"><span data-stu-id="a80dc-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="a80dc-108">Faceți clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="a80dc-108">Click **Search**.</span></span>

<span data-ttu-id="a80dc-109">În rezultate, selectați o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="a80dc-109">In the results, select an audit record.</span></span> <span data-ttu-id="a80dc-110">În flyout detalii, faceți clic pe **mai multe informații**.</span><span class="sxs-lookup"><span data-stu-id="a80dc-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="a80dc-111">Sunt afișate informații despre setările regulii Inbox în câmpul **parametri** .</span><span class="sxs-lookup"><span data-stu-id="a80dc-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="a80dc-112">Pentru mai multe informații, consultați [determinarea dacă un utilizator a creat o regulă de Inbox](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="a80dc-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
