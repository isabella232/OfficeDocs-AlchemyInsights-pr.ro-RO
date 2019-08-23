---
title: Identifica activitatea de regulă inbox în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539185"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="5f354-102">Identifica activitatea de regulă inbox în jurnalele de auditare</span><span class="sxs-lookup"><span data-stu-id="5f354-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="5f354-103">Utilizaţi căutare de jurnal audit în Office 365 securitate & centru de conformitate pentru a vizualiza evenimente de regulă inbox (crearea, modificarea şi ştergerea regulilor inbox).</span><span class="sxs-lookup"><span data-stu-id="5f354-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="5f354-104">Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5f354-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5f354-105">Du-te la **Căutare** > pagina de**Căutare de jurnalul de Audit** .</span><span class="sxs-lookup"><span data-stu-id="5f354-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="5f354-106">Selectaţi intervalul de date în câmpurile **data de început** şi **data de sfârşit** .</span><span class="sxs-lookup"><span data-stu-id="5f354-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="5f354-107">În cadrul **Activităţilor de cutie poştală Exchange**, verificaţi câmpul de **activităţi** este setat la **regula de inbox New-InboxRule creare/modificare/activare/dezactivare**.</span><span class="sxs-lookup"><span data-stu-id="5f354-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="5f354-108">Faceţi clic pe **Căutare**.</span><span class="sxs-lookup"><span data-stu-id="5f354-108">Click **Search**.</span></span>

<span data-ttu-id="5f354-109">În rezultate, selectaţi o înregistrare de audit.</span><span class="sxs-lookup"><span data-stu-id="5f354-109">In the results, select an audit record.</span></span> <span data-ttu-id="5f354-110">În fișă de detalii, faceţi clic pe **Mai multe informaţii**.</span><span class="sxs-lookup"><span data-stu-id="5f354-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="5f354-111">Informații despre setările de regulă inbox este afişat în câmpul de **parametri** .</span><span class="sxs-lookup"><span data-stu-id="5f354-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="5f354-112">Pentru informaţii suplimentare, consultaţi [determină în cazul în care un utilizator a creat o regulă inbox](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="5f354-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
