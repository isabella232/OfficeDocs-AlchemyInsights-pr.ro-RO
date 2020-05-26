---
title: Adresarea echipelor de conectare eroare AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357872"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="461a5-102">Adresarea echipelor de conectare eroare AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="461a5-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="461a5-103">Atunci când vă conectați la Microsoft Teams, este posibil să primiți eroarea: **Ne pare rău, dar avem probleme cu semnarea în AADSTS9000411: Solicitarea nu este formatat corect. Parametrul "login_hint" este duplicat.**</span><span class="sxs-lookup"><span data-stu-id="461a5-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="461a5-104">Pentru a rezolva această problemă, asigurați-vă că clienții Microsoft Teams sunt actualizate.</span><span class="sxs-lookup"><span data-stu-id="461a5-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="461a5-105">Pentru mai multe informații despre actualizarea clientului, consultați [Actualizarea Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="461a5-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="461a5-106">Dacă nu se poate actualiza clientul dintr-un anumit motiv, deconectarea clientului va șterge majoritatea datelor memorate în cache.</span><span class="sxs-lookup"><span data-stu-id="461a5-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="461a5-107">Cu toate acestea, dacă aveți în continuare probleme după logoff/logon, închideți Echipe și goliți memoria cache a clientului procedând astfel:</span><span class="sxs-lookup"><span data-stu-id="461a5-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="461a5-108">Închideți Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="461a5-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="461a5-109">Accesați: %appdata%\microsoft\teams și ștergeți toate fișierele.</span><span class="sxs-lookup"><span data-stu-id="461a5-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="461a5-110">Redeschideți Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="461a5-110">Reopen Microsoft Teams.</span></span>
