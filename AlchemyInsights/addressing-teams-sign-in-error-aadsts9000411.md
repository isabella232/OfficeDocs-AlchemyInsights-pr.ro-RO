---
title: Adresarea erorii de conectare Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821999"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="9c4d1-102">Adresarea erorii de conectare Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="9c4d1-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="9c4d1-103">Atunci când vă conectați la Microsoft Teams, este posibil să primiți eroarea: Ne pare rău, dar avem probleme cu conectarea dvs. la **AADSTS9000411: Solicitarea nu este formatată corect. Parametrul "login_hint" este dublat.**</span><span class="sxs-lookup"><span data-stu-id="9c4d1-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="9c4d1-104">Pentru a rezolva această problemă, asigurați-vă că clienții Microsoft Teams sunt actualizați.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="9c4d1-105">Pentru mai multe informații despre actualizarea clientului, consultați [Actualizarea Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="9c4d1-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="9c4d1-106">Dacă nu puteți actualiza clientul dintr-un anumit motiv, deconectarea de la client va șterge majoritatea datelor memorate în cache.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="9c4d1-107">Cu toate acestea, dacă aveți încă probleme după logoff/logon, închideți Teams și goliți memoria cache a clientului, în modul următor:</span><span class="sxs-lookup"><span data-stu-id="9c4d1-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="9c4d1-108">Închideți Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="9c4d1-109">Accesați: %appdata%\microsoft\teams și ștergeți toate fișierele.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="9c4d1-110">Redeschideți Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-110">Reopen Microsoft Teams.</span></span>
