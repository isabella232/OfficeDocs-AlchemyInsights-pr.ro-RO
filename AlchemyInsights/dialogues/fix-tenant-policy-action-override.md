---
title: Remedierea politicii de entitate găzduită (înlocuire de acțiune)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695696"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="f1b8a-102">Remedierea politicii de entitate găzduită (înlocuire de acțiune)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="f1b8a-103">O politică anti-spam din entitatea găzduită a afectat acest mesaj.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="f1b8a-104">Pentru a revizui politica, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="f1b8a-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="f1b8a-105">Accesați centrul de [conformitate Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143), apoi accesați Politica de **gestionare a amenințărilor**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="f1b8a-106">Verificați dacă sursa de **politică** indică următoarele:  **Adăugare-XHeader/ModifySubject/redirecționare/Ștergere/niciun mesaj de acțiune/CCI**</span><span class="sxs-lookup"><span data-stu-id="f1b8a-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="f1b8a-107">Dacă da, pe fila **particularizat** , Verificați setările politicii care au afectat mesajul.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="f1b8a-108">Este posibil ca **setările standard** aplicate pentru toți clienții Exchange Online Protection să fi afectat mesajul.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="f1b8a-109">Pentru mai multe informații despre configurarea politicilor de filtrare antispam, consultați [Configurarea politicilor de filtrare antispam](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
