---
title: Remedierea politicii de conexiune
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695885"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="b31e2-102">Remedierea politicii de conexiune</span><span class="sxs-lookup"><span data-stu-id="b31e2-102">Fix connection policy</span></span>

<span data-ttu-id="b31e2-103">Mesajul de e-mail a fost marcat în siguranță și livrat în inboxul utilizatorului, deoarece adresa IP de trimitere a fost marcată în siguranță în Politica de filtrare a conexiunii.</span><span class="sxs-lookup"><span data-stu-id="b31e2-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="b31e2-104">Pentru a revizui politica, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="b31e2-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="b31e2-105">Accesați centrul de [conformitate Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143), apoi accesați Politica de **gestionare a amenințărilor**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="b31e2-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="b31e2-106">Pe fila **particularizat** , selectați Politica de **filtrare a conexiunii**, apoi selectați **Editare politică**.</span><span class="sxs-lookup"><span data-stu-id="b31e2-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="b31e2-107">Revizuiți lista de **permisiuni IP** .</span><span class="sxs-lookup"><span data-stu-id="b31e2-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="b31e2-108">Vedeți dacă este activată **lista sigură** .</span><span class="sxs-lookup"><span data-stu-id="b31e2-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b31e2-109">Microsoft se abonează la sursele terților de expeditori de încredere.</span><span class="sxs-lookup"><span data-stu-id="b31e2-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="b31e2-110">Dacă este activată **lista sigură** , acești expeditori de încredere nu sunt marcați din greșeală ca spam.</span><span class="sxs-lookup"><span data-stu-id="b31e2-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="b31e2-111">Vă recomandăm să selectați această opțiune, deoarece va reduce numărul de fals pozitive (corespondență bună clasificat ca spam) pe care îl primiți.</span><span class="sxs-lookup"><span data-stu-id="b31e2-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
