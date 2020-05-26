---
title: 618 Politica de partajare a calendarului
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373011"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="810e3-102">Eroare de politică la partajarea unui calendar</span><span class="sxs-lookup"><span data-stu-id="810e3-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="810e3-103">Efectuați una dintre următoarele acțiuni, în funcție de situația dvs.:</span><span class="sxs-lookup"><span data-stu-id="810e3-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="810e3-104">Conectați-vă la Exchange Online utilizând Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="810e3-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="810e3-105">Pentru mai multe informații, consultați [Conectarea la Exchange Online utilizând Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="810e3-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="810e3-106">Pe serverul local, deschideți Componentă de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="810e3-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="810e3-107">Determinați politica de partajare care este atribuită utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="810e3-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="810e3-108">Pentru aceasta, executați următoarea comandă și notați politica returnată:</span><span class="sxs-lookup"><span data-stu-id="810e3-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="810e3-109">Actualizați politica de partajare pentru utilizator.</span><span class="sxs-lookup"><span data-stu-id="810e3-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="810e3-110">Pentru a proceda astfel, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="810e3-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="810e3-111">Deschideți centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="810e3-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="810e3-112">Faceți clic pe **Organizație**, apoi faceți dublu clic pe politica atribuită utilizatorului sub **Partajare individuală**.</span><span class="sxs-lookup"><span data-stu-id="810e3-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="810e3-113">Aceasta este politica care a fost returnată în pasul 2.</span><span class="sxs-lookup"><span data-stu-id="810e3-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="810e3-114">Pe pagina Regulă partajare, selectați nivelul de partajare a calendarului pe care doriți să îl permiteți sub **Specificați ce informații doriți să partajați;** faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="810e3-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="810e3-115">Pentru mai multe informații, [consultați: "Politica nu permite acordarea permisiunilor la acest nivel la unul sau mai multe dintre destinatarii" eroare atunci când utilizatorul încearcă să partajeze calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="810e3-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
