---
title: Protecție împotriva atacului prin puncte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037176"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="2a422-102">Protecție împotriva atacului prin puncte</span><span class="sxs-lookup"><span data-stu-id="2a422-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="2a422-103">Mesajele de completare sunt rapoarte de nelivrare (denumite și mesaje rapoarte NDR sau sarituri) pe care le primiți pentru mesajele pe care nu le-ați trimis.</span><span class="sxs-lookup"><span data-stu-id="2a422-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="2a422-104">Spammeri Forge (spoof) de **la:** adresa mesajelor lor și folosesc deseori adrese de e-mail reale pentru a-și acorda credibilitate mesajelor.</span><span class="sxs-lookup"><span data-stu-id="2a422-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="2a422-105">Așadar, atunci când autorii de spam trimit în mod inevitabil mesaje către destinatari inexistenți, serverul de e-mail de destinație este în esență păcălit să returneze mesajul nelivrat într-un NDR către expeditorul falsificat în adresa **de la:** .</span><span class="sxs-lookup"><span data-stu-id="2a422-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="2a422-106">Informații suplimentare pot fi găsite în [puncte de completare în EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="2a422-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="2a422-107">**Activarea protecției prin puncte**</span><span class="sxs-lookup"><span data-stu-id="2a422-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="2a422-108">Pentru a activa protecția prin puncte, urmați calea de mai jos.</span><span class="sxs-lookup"><span data-stu-id="2a422-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="2a422-109">**protection.office.com > gestionarea amenințărilor > politica > antispam > selectați Politica de filtrare antispam și politica de editare > proprietățile spam > Marcați ca spam > NDR prin mesaje > setați-l la "activat"**</span><span class="sxs-lookup"><span data-stu-id="2a422-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="2a422-110">Dacă credeți că un cont a fost compromis, consultați următoarele:</span><span class="sxs-lookup"><span data-stu-id="2a422-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="2a422-111">Răspunsul la un cont de E-mail compromis</span><span class="sxs-lookup"><span data-stu-id="2a422-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="2a422-112">Eliminarea utilizatorilor blocați din portalul utilizatori restricționați din Office 365</span><span class="sxs-lookup"><span data-stu-id="2a422-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



