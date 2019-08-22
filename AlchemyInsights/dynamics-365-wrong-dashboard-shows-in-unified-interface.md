---
title: Dynamics 365 - tabloul de bord greşit arată în interfaţă unificată Dynamics 365
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528563"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="4922e-102">Tabloul de bord greşit arată în interfaţă unificată Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="4922e-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="4922e-103">Există mai multe motive de ce pot vedea un tablou de bord diferite decât cea pe care aţi aştepta:</span><span class="sxs-lookup"><span data-stu-id="4922e-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="4922e-104">Utilizatorul a stabilit un tablou de bord utilizator implicit</span><span class="sxs-lookup"><span data-stu-id="4922e-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="4922e-105">De obicei poate identifica un utilizator implicit tabloul de bord este situat în cazul în care butonul **Setat ca implicit** nu arată în bara de comenzi tabloul de bord.</span><span class="sxs-lookup"><span data-stu-id="4922e-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="4922e-106">Tabloul de bord utilizator implicit va suprascrie toate alte dashboards implicit, chiar dacă utilizatorul implicit tabloul de bord nu este în app curent.</span><span class="sxs-lookup"><span data-stu-id="4922e-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="4922e-107">Utilizaţi următoarele workaround pentru a demarca implicit tabloul de bord.</span><span class="sxs-lookup"><span data-stu-id="4922e-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="4922e-108">Creați un nou tablou de bord personale.</span><span class="sxs-lookup"><span data-stu-id="4922e-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="4922e-109">Setaţi ca nou tablou de bord utilizator implicit.</span><span class="sxs-lookup"><span data-stu-id="4922e-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="4922e-110">Şterge acest tablou de bord.</span><span class="sxs-lookup"><span data-stu-id="4922e-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="4922e-111">Tabloul de bord este situat în sitemap</span><span class="sxs-lookup"><span data-stu-id="4922e-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="4922e-112">Poate aţi setat o organizaţie implicit tabloul de bord prin selectarea un tablou de bord şi alegerea 'Setat ca Default' sub 'Particularizarea sistemului'.</span><span class="sxs-lookup"><span data-stu-id="4922e-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="4922e-113">Dar tabloul de bord definite în sitemap proiectantul vor avea prioritate peste acest tablou de bord, în cazul în care utilizatorul are acces la aceasta.</span><span class="sxs-lookup"><span data-stu-id="4922e-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="4922e-114">Pentru ca utilizatorii vedea tabloul de bord pe care aţi setat ca implicit organizaţie, aveţi posibilitatea să fie:</span><span class="sxs-lookup"><span data-stu-id="4922e-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="4922e-115">Stabilit că tabloul de bord în sitemap</span><span class="sxs-lookup"><span data-stu-id="4922e-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="4922e-116">Elimina accesul la tabloul de bord sitemap definite pentru acei utilizatori</span><span class="sxs-lookup"><span data-stu-id="4922e-116">Remove access to the sitemap defined dashboard for those users</span></span>
