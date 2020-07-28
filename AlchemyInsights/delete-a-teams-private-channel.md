---
title: Ștergerea unui canal privat Echipe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439917"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="a82fd-102">Ștergerea unui canal privat Echipe</span><span class="sxs-lookup"><span data-stu-id="a82fd-102">Delete a Teams private channel</span></span>

<span data-ttu-id="a82fd-103">Microsoft este conștient de o problemă la ștergerea unui canal privat Teams dacă aveți politicile de retenție SharePoint activate pentru site-ul SharePoint subiacent.</span><span class="sxs-lookup"><span data-stu-id="a82fd-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="a82fd-104">Microsoft lucrează la o remediere.</span><span class="sxs-lookup"><span data-stu-id="a82fd-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="a82fd-105">Între timp, puteți utiliza următoarele soluții pentru a șterge canalul privat.</span><span class="sxs-lookup"><span data-stu-id="a82fd-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="a82fd-106">**Excludeți colecția de echipă/site din politica de retenție Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="a82fd-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="a82fd-107">Accesați portalul de administrare Office 365 și selectați **Afișare totală** în panoul de navigare din stânga.</span><span class="sxs-lookup"><span data-stu-id="a82fd-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="a82fd-108">Sub **Centre de administrare**, accesați Politica de prevenire a **Security & Compliance**  >  **pierderilor de date**de &  >  **conformitate**.</span><span class="sxs-lookup"><span data-stu-id="a82fd-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="a82fd-109">Identificați orice politică care se aplică site-urilor Sharepoint și modificați politica astfel încât site-ul Sharepoint pentru echipa care conține canalul privat SĂ NU fie inclus în politica de retenție.</span><span class="sxs-lookup"><span data-stu-id="a82fd-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="a82fd-110">Salvează politica.</span><span class="sxs-lookup"><span data-stu-id="a82fd-110">Save the policy.</span></span>
    <span data-ttu-id="a82fd-111">Poate dura până la 24 de ore pentru ca setările de politică să intre în vigoare.</span><span class="sxs-lookup"><span data-stu-id="a82fd-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="a82fd-112">După ce site-ul a fost exclus, puteți șterge canalul privat.</span><span class="sxs-lookup"><span data-stu-id="a82fd-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="a82fd-113">Este ***posibil*** să puteți șterge canalul privat utilizând Microsoft Teams pe dispozitivul Android.</span><span class="sxs-lookup"><span data-stu-id="a82fd-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="a82fd-114">Pentru informații SharePoint corelate, consultați [Imposibil de șters elemente din SharePoint Online sau OneDrive pentru business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="a82fd-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>