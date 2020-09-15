---
title: Dinamica 365-afișează un tablou de bord incorect în interfața unificată Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711287"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="be8e4-102">Afișează un tablou de bord greșit în interfața unificată Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="be8e4-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="be8e4-103">Există mai multe motive pentru care este posibil să vedeți un tablou de bord diferit de cel la care vă așteptați:</span><span class="sxs-lookup"><span data-stu-id="be8e4-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="be8e4-104">Utilizatorul a setat un tablou de bord implicit pentru utilizator</span><span class="sxs-lookup"><span data-stu-id="be8e4-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="be8e4-105">De obicei, puteți identifica un tablou de bord implicit pentru utilizator este setat dacă butonul **Stabilire ca implicit** nu se afișează în bara de comenzi tablou de bord.</span><span class="sxs-lookup"><span data-stu-id="be8e4-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="be8e4-106">Tabloul de bord implicit pentru utilizator va anula toate celelalte tablouri de bord implicite, chiar dacă tabloul de bord implicit al utilizatorului nu se află în aplicația curentă.</span><span class="sxs-lookup"><span data-stu-id="be8e4-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="be8e4-107">Utilizați următoarea soluție pentru a-i unse tabloul de bord implicit.</span><span class="sxs-lookup"><span data-stu-id="be8e4-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="be8e4-108">Creați un tablou de bord personal nou.</span><span class="sxs-lookup"><span data-stu-id="be8e4-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="be8e4-109">Setați tabloul de bord nou ca implicit pentru utilizator.</span><span class="sxs-lookup"><span data-stu-id="be8e4-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="be8e4-110">Ștergeți tabloul de bord.</span><span class="sxs-lookup"><span data-stu-id="be8e4-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="be8e4-111">Tabloul de bord este setat în Sitemap</span><span class="sxs-lookup"><span data-stu-id="be8e4-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="be8e4-112">Este posibil să fi setat un tablou de bord implicit pentru organizație selectând un tablou de bord și alegând "stabilire ca implicit" sub "Particularizare sistem".</span><span class="sxs-lookup"><span data-stu-id="be8e4-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="be8e4-113">Dar tabloul de bord definit în proiectantul Sitemap-urilor va prevala asupra acestui tablou de bord, dacă utilizatorul are acces la acesta.</span><span class="sxs-lookup"><span data-stu-id="be8e4-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="be8e4-114">Pentru ca utilizatorii să vadă tabloul de bord pe care l-ați setat ca implicit al Organizației, puteți fie:</span><span class="sxs-lookup"><span data-stu-id="be8e4-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="be8e4-115">Setarea tabloului de bord în Sitemap</span><span class="sxs-lookup"><span data-stu-id="be8e4-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="be8e4-116">Eliminarea accesului la tabloul de bord definit al Sitemap pentru acei utilizatori</span><span class="sxs-lookup"><span data-stu-id="be8e4-116">Remove access to the sitemap defined dashboard for those users</span></span>
