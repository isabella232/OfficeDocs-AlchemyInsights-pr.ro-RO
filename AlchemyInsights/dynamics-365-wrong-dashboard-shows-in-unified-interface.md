---
title: Dynamics 365-greșit tabloul de bord arată în Dynamics 365 interfață unificată
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528563"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="3a3bd-102">Greșit tabloul de bord arată în Dynamics 365 interfață unificată</span><span class="sxs-lookup"><span data-stu-id="3a3bd-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="3a3bd-103">Există mai multe motive pentru care este posibil să vedeți un tablou de bord diferit de cel la care vă așteptați:</span><span class="sxs-lookup"><span data-stu-id="3a3bd-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="3a3bd-104">Utilizatorul a setat un tablou de bord implicit de utilizator</span><span class="sxs-lookup"><span data-stu-id="3a3bd-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="3a3bd-105">De obicei, aveți posibilitatea să identificați un tablou de bord implicit de utilizator este setată dacă butonul **set as default** nu se afișează în bara de comenzi a tabloului de bord.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="3a3bd-106">Tabloul de bord implicit de utilizator va suprascrie toate celelalte tablouri de bord implicite, chiar dacă tabloul de bord implicit al utilizatorului nu este în aplicația curentă.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="3a3bd-107">Utilizați următoarea soluție pentru a deseta tabloul de bord implicit.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="3a3bd-108">Creați un tablou de bord personal nou.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="3a3bd-109">Setați tabloul de bord nou ca implicit de utilizator.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="3a3bd-110">Ștergeți tabloul de bord.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="3a3bd-111">Tabloul de bord este setat în Sitemap</span><span class="sxs-lookup"><span data-stu-id="3a3bd-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="3a3bd-112">Este posibil să fi setat un tablou de bord implicit de organizație selectând un tablou de bord și alegând "setați ca implicit" sub "Particularizare sistem".</span><span class="sxs-lookup"><span data-stu-id="3a3bd-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="3a3bd-113">Dar tabloul de bord definit în proiectantul de Sitemap va avea prioritate față de acest tablou de bord, dacă utilizatorul are acces la acesta.</span><span class="sxs-lookup"><span data-stu-id="3a3bd-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="3a3bd-114">Pentru ca utilizatorii să vadă tabloul de bord pe care l-ați setat ca implicit al Organizației, puteți fie:</span><span class="sxs-lookup"><span data-stu-id="3a3bd-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="3a3bd-115">Setați tabloul de bord în Sitemap</span><span class="sxs-lookup"><span data-stu-id="3a3bd-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="3a3bd-116">Eliminați accesul la tabloul de bord definit de Sitemap pentru acei utilizatori</span><span class="sxs-lookup"><span data-stu-id="3a3bd-116">Remove access to the sitemap defined dashboard for those users</span></span>
