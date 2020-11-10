---
title: Comentarii la elementele din listă
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982560"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="92cf5-102">Comentarii la elementele din listă</span><span class="sxs-lookup"><span data-stu-id="92cf5-102">Comments on List items</span></span>

<span data-ttu-id="92cf5-103">Utilizatorii vor putea în curând să adauge și să șteargă comentarii în elementele din listă.</span><span class="sxs-lookup"><span data-stu-id="92cf5-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="92cf5-104">Utilizatorii pot să vizualizeze toate comentariile unui element de listă și să filtreze între vizualizări care afișează comentariile sau activitatea asociate unui element.</span><span class="sxs-lookup"><span data-stu-id="92cf5-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="92cf5-105">**Temporizare** :</span><span class="sxs-lookup"><span data-stu-id="92cf5-105">**Timing** :</span></span>

<span data-ttu-id="92cf5-106">**Lansare specifică** : roll progresiv în Mid-octombrie și se așteaptă să se finalizeze până la mijlocul lunii noiembrie</span><span class="sxs-lookup"><span data-stu-id="92cf5-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="92cf5-107">**Ediție standard** : roll treptat la mijlocul lunii noiembrie și se așteaptă să se finalizeze până la începutul lunii decembrie</span><span class="sxs-lookup"><span data-stu-id="92cf5-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="92cf5-108">**Implementare** : lansare specifică pentru întreaga organizație</span><span class="sxs-lookup"><span data-stu-id="92cf5-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="92cf5-109">Utilizatorii trebuie să rețină următoarele înainte de a putea adăuga și șterge comentarii:</span><span class="sxs-lookup"><span data-stu-id="92cf5-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="92cf5-110">Comentarii urmați setările de permisiune inerente în SharePoint.</span><span class="sxs-lookup"><span data-stu-id="92cf5-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="92cf5-111">Listele clasice care nu sunt construite încă pentru a se afișa în interfețele moderne de utilizator, cum ar fi listele de activități, nu vor avea această caracteristică de comentare.</span><span class="sxs-lookup"><span data-stu-id="92cf5-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="92cf5-112">Comentarea în listele din teams nu este disponibilă în această ediție.</span><span class="sxs-lookup"><span data-stu-id="92cf5-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="92cf5-113">Comentariile nu sunt indexate de căutare.</span><span class="sxs-lookup"><span data-stu-id="92cf5-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="92cf5-114">Administratorii pot dezactiva această caracteristică la nivel de organizație, modificând parametrul **CommentsOnListItemsDisabled** din cmdletul **Set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="92cf5-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="92cf5-115">În prezent, nu este posibil să dezactivați comentarea la site sau la nivelul listei.</span><span class="sxs-lookup"><span data-stu-id="92cf5-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="92cf5-116">Sperăm să avem acele controale într-o actualizare ulterioară, probabil în primul trimestru 2021.</span><span class="sxs-lookup"><span data-stu-id="92cf5-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
