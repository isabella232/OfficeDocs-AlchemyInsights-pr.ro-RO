---
title: Pictograma Calendar nu se afișează în clientul Microsoft teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583924"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="c43b7-102">Pictograma Calendar nu se afișează în clientul Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="c43b7-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="c43b7-103">Fila **Calendar** din teams necesită acces la o cutie poștală Exchange prin Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="c43b7-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="c43b7-104">Cutia poștală Exchange poate fi online sau locală.</span><span class="sxs-lookup"><span data-stu-id="c43b7-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="c43b7-105">Pentru utilizatorii online care nu văd fila **Calendar** , asigurați-vă că [sunt autorizați pentru o cutie poștală Exchange Online și că este activată cutia poștală](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="c43b7-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="c43b7-106">Dacă utilizatorii sunt conectați local, trebuie să confirmați că configurația hibridă este sănătoasă.</span><span class="sxs-lookup"><span data-stu-id="c43b7-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="c43b7-107">Utilizați [Expertul de Configurare Hibridă ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pentru a depana.</span><span class="sxs-lookup"><span data-stu-id="c43b7-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="c43b7-108">Rețineți că [Teams necesită Exchange 2016 CU3 sau o versiune mai recentă](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="c43b7-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="c43b7-109">Pentru mai multe informații și pași de depanare, consultați [Depanarea problemelor de interacțiune Microsoft teams și Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="c43b7-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
