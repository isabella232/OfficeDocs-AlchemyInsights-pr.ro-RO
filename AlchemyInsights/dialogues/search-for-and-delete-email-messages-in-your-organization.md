---
title: Căutarea și ștergerea mesajelor de e-mail din organizație
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525439"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="48eb1-102">Căutarea și ștergerea mesajelor de e-mail din organizație</span><span class="sxs-lookup"><span data-stu-id="48eb1-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="48eb1-103">Urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="48eb1-103">Follow these steps:</span></span>

1. <span data-ttu-id="48eb1-104">Dacă nu sunteți administrator global, pentru a căuta mesaje, contul trebuie adăugat la **grupul de roluri EDiscovery Manager** sau la rolul de **gestionare a căutării conformității**.</span><span class="sxs-lookup"><span data-stu-id="48eb1-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="48eb1-105">Pentru a șterge mesaje, va trebui să vă asociați **grupului de roluri pentru gestionarea organizației** sau **rolul de gestionare a căutării și eliminării**.</span><span class="sxs-lookup"><span data-stu-id="48eb1-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="48eb1-106">Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate & conformitate.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="48eb1-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="48eb1-107">[Creați o căutare de conținut](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul de șters.</span><span class="sxs-lookup"><span data-stu-id="48eb1-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="48eb1-108">[Conectați-vă la Security & Conformity Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="48eb1-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="48eb1-109">Dacă utilizați Mae, consultați aceste instrucțiuni: [conectarea la Security & la centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="48eb1-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="48eb1-110">Ștergeți mesajul: rulează `New-ComplianceSearchAction` cmdletul pentru a șterge mesajul.</span><span class="sxs-lookup"><span data-stu-id="48eb1-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="48eb1-111">Mesajele șterse sunt mutate în folderul Elemente recuperabile ale unui utilizator.</span><span class="sxs-lookup"><span data-stu-id="48eb1-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="48eb1-112">Pentru o comandă exemplu, consultați [Pasul 3: ștergerea mesajului.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="48eb1-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
