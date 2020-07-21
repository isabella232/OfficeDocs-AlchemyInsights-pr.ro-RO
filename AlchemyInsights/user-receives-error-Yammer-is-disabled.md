---
title: Utilizatorul primește eroarea AADSTS7000112 Yammer este dezactivat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198374"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="05958-102">Utilizatorul primește eroarea AADSTS7000112 Yammer este dezactivat</span><span class="sxs-lookup"><span data-stu-id="05958-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="05958-103">Dacă primiți eroarea "AADSTS7000112: Aplicația '00000005-0000-0ff1-ce00-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000</span><span class="sxs-lookup"><span data-stu-id="05958-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="05958-104">Este posibil ca un administrator să fi dezactivat principalul serviciului pentru a bloca accesul la Yammer.</span><span class="sxs-lookup"><span data-stu-id="05958-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="05958-105">Dezactivarea principalului serviciului nu este recomandată și poate provoca probleme suplimentare.</span><span class="sxs-lookup"><span data-stu-id="05958-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="05958-106">Pentru mai multe informații despre abordarea acceptată pentru a bloca accesul utilizatorilor la Yammer, consultați [Dezactivarea accesului Yammer pentru utilizatorii Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="05958-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="05958-107">Pentru a corecta această problemă în portalul Azure și a restabili accesul utilizatorului la Yammer:</span><span class="sxs-lookup"><span data-stu-id="05958-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="05958-108">Deschideți pagina Azure Active Directory și selectați **Aplicații enterprise** sub **Gestionare** în panoul de navigare din stânga.</span><span class="sxs-lookup"><span data-stu-id="05958-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="05958-109">Tastați **Office 365 Yammer** în caseta de căutare și selectați numele aplicației pentru a deschide setările.</span><span class="sxs-lookup"><span data-stu-id="05958-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="05958-110">Selectați **Proprietăți** sub **Gestionare** în panoul de navigare din stânga.</span><span class="sxs-lookup"><span data-stu-id="05958-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="05958-111">Setați valoarea **Activat pentru ca utilizatorii să se conecteze?** **Yes** **Save**</span><span class="sxs-lookup"><span data-stu-id="05958-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="05958-112">Conectați-vă din nou la Yammer.</span><span class="sxs-lookup"><span data-stu-id="05958-112">Sign in to Yammer again.</span></span> <span data-ttu-id="05958-113">S-ar putea să trebuiți să ștergeți cookie-urile.</span><span class="sxs-lookup"><span data-stu-id="05958-113">You might need to clear cookies.</span></span>

<span data-ttu-id="05958-114">Alternativ, executați comenziLe PowerShell pentru a seta valoarea.</span><span class="sxs-lookup"><span data-stu-id="05958-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="05958-115">Pentru mai multe informații, consultați [eroarea "Ne pare rău, dar întâmpinam probleme la conectare" atunci când faceți clic pe dala Yammer din Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="05958-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 