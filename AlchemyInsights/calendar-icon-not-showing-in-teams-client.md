---
title: Pictograma Calendar nu e afișată în clientul Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932197"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="1038a-102">Pictograma Calendar nu e afișată în clientul Teams</span><span class="sxs-lookup"><span data-stu-id="1038a-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="1038a-103">Fila Calendar din Teams necesită acces la o cutie poștală Exchange via Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="1038a-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="1038a-104">Cutia poștală Exchange poate fi Online sau La-Locație.</span><span class="sxs-lookup"><span data-stu-id="1038a-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="1038a-105">Pentru utilizatorii Online care nu văd Fila Calendar, asigurați-vă că acestea [sunt licențiate pentru o cutie poștală Exchange Online, iar cutia poștală este activată](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="1038a-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="1038a-106">Dacă un utilizator are o cutie poștală validă în Exchange Online, dar tot nu poate vedea Fila Calendar, este posibil să întâmpinați o problemă de rețea.</span><span class="sxs-lookup"><span data-stu-id="1038a-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="1038a-107">Utilizați [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) și rulați **Testele de Conectivitate Microsoft Exchange Web Services** pentru utilizatorul afectat.</span><span class="sxs-lookup"><span data-stu-id="1038a-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="1038a-108">În cele din urmă, verificați aplicațiile [Teams Apps - politicile de instalare a aplicațiilor](https://admin.teams.microsoft.com/policies/app-setup) pentru a vă asigura că aplicația Calendar nu a fost eliminată din politica aplicată utilizatorului (cel mai probabil, **Global (implicit la nivel de Organizație)**.</span><span class="sxs-lookup"><span data-stu-id="1038a-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="1038a-109">Dacă utilizatorii dvs. au domiciliul La-Locație, trebuie să confirmați că este sănătoasă configurația hibridă.</span><span class="sxs-lookup"><span data-stu-id="1038a-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="1038a-110">Utilizați [Expertul de Configurare Hibridă ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pentru a depana.</span><span class="sxs-lookup"><span data-stu-id="1038a-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="1038a-111">Rețineți că [Teams necesită Exchange 2016 CU3 sau o versiune mai recentă](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="1038a-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
