---
title: Cutia poștală de arhivă este aproape completă
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974661"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="74400-102">Cutia poștală de arhivă este aproape completă</span><span class="sxs-lookup"><span data-stu-id="74400-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="74400-103">Dacă utilizatorul primește avertismentul; **Cutia poștală de arhivă este aproape completă** sau trebuie să măriți dimensiunea cutiei poștale de arhivă, iată câteva sfaturi:</span><span class="sxs-lookup"><span data-stu-id="74400-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="74400-104">Dacă utilizatorului i se atribuie un plan Exchange Online 1, faceți upgrade la licența **Exchange Online Plan 2** pentru a mări dimensiunea de la 50 GB la 100 GB.</span><span class="sxs-lookup"><span data-stu-id="74400-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="74400-105">Dacă utilizatorul este deja atribuit oricare dintre următoarele: **Exchange Online Plan 2** sau un Exchange Online plan 1 cu un program de completare Arhivare Exchange Online, utilizați pașii de mai jos pentru a activa Arhivarea automată a extinderii:.</span><span class="sxs-lookup"><span data-stu-id="74400-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="74400-106">[Conectați-vă la Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="74400-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="74400-107">Rulează următorul poate configura utilizând pentru utilizator:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="74400-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="74400-108">Rularea următoarelor poate configura utilizând pentru a confirma că este activată pentru utilizator:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="74400-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="74400-109">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="74400-109">For more information see:</span></span>

- [<span data-ttu-id="74400-110"> Activarea Arhivării nelimitate-ajutor pentru administratori-Microsoft 365 Conformity | Documente Microsoft</span><span class="sxs-lookup"><span data-stu-id="74400-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="74400-111">Limitele Exchange Online-descrierile serviciului | Documente Microsoft</span><span class="sxs-lookup"><span data-stu-id="74400-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="74400-112">Upgrade-ul la un alt plan de afaceri | Documente Microsoft</span><span class="sxs-lookup"><span data-stu-id="74400-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

