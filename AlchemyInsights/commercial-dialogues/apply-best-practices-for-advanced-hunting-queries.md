---
title: Aplicarea celor mai bune practici pentru interogările complexe de vânătoare
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749546"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="17dc0-102">Aplicarea celor mai bune practici pentru interogările complexe de vânătoare</span><span class="sxs-lookup"><span data-stu-id="17dc0-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="17dc0-103">Pentru a obține rezultate mai rapid și pentru a evita expirarea în timp ce rulați interogări complexe, aplicați aceste bune practici:</span><span class="sxs-lookup"><span data-stu-id="17dc0-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="17dc0-104">Atunci când încercați interogări noi, utilizați întotdeauna o limită, pentru a evita să obțineți seturi de rezultate extrem de mari.</span><span class="sxs-lookup"><span data-stu-id="17dc0-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="17dc0-105">De asemenea, utilizați `count` pentru a face o evaluare inițială a dimensiunii setului de rezultate.</span><span class="sxs-lookup"><span data-stu-id="17dc0-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="17dc0-106">Utilizați mai întâi filtrele de timp.</span><span class="sxs-lookup"><span data-stu-id="17dc0-106">Use time filters first.</span></span> <span data-ttu-id="17dc0-107">În mod ideal, limitați interogările la șapte zile.</span><span class="sxs-lookup"><span data-stu-id="17dc0-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="17dc0-108">La începutul unei interogări, imediat după filtrul de timp, adăugați filtrele de așteptat pentru a elimina majoritatea datelor.</span><span class="sxs-lookup"><span data-stu-id="17dc0-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="17dc0-109">Atunci când căutați jetoane complete, utilizați operatorul, `has` mai degrabă decât `contains` .</span><span class="sxs-lookup"><span data-stu-id="17dc0-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="17dc0-110">Rulează o căutare pe o anumită coloană, mai degrabă decât pe toate coloanele.</span><span class="sxs-lookup"><span data-stu-id="17dc0-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="17dc0-111">Atunci când vă asociați la tabele, specificați mai întâi tabelul cu mai puține rânduri.</span><span class="sxs-lookup"><span data-stu-id="17dc0-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="17dc0-112">`project` numai coloanele necesare din tabelele pe care le-ați asociat.</span><span class="sxs-lookup"><span data-stu-id="17dc0-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="17dc0-113">Pentru a afla mai multe, consultați [cele mai bune practici pentru interogarea de vânătoare complexe](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="17dc0-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
