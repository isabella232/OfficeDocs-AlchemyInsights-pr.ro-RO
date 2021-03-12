---
title: Remedierea regulilor de transport
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750577"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="bcd63-102">Remedierea regulilor de transport</span><span class="sxs-lookup"><span data-stu-id="bcd63-102">Fix transport rules</span></span>

<span data-ttu-id="bcd63-103">O regulă de flux de corespondență particularizată A afectat acest mesaj.</span><span class="sxs-lookup"><span data-stu-id="bcd63-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="bcd63-104">Pentru a revizui regula exactă, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="bcd63-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="bcd63-105">În rezultatele remiterii, sub **informații suplimentare**, notați **GUID** -ul sau **numele politicii**.</span><span class="sxs-lookup"><span data-stu-id="bcd63-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="bcd63-106">Lansați componenta de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcd63-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="bcd63-107">Pentru mai multe informații, consultați [Deschideți componenta de administrare Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="bcd63-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="bcd63-108">Rularea acestei comenzi (utilizând GUID-ul de la prezentarea dvs.):  **Get-TransportRule-Identity "GUID" | FL \* Descriere**\*</span><span class="sxs-lookup"><span data-stu-id="bcd63-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="bcd63-109">Revizuiți Descrierea pentru a vedea condițiile configurate care au afectat mesajul.</span><span class="sxs-lookup"><span data-stu-id="bcd63-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="bcd63-110">Pentru a afla mai multe, consultați [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="bcd63-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
