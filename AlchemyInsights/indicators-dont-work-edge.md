---
title: Indicatorii nu funcționează utilizând browserul Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676464"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="24e92-102">Indicatorii nu funcționează utilizând browserul Edge</span><span class="sxs-lookup"><span data-stu-id="24e92-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="24e92-103">După ce ați creat un indicator, acesta nu este onorat de Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="24e92-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="24e92-104">Pentru mai multe informații, [consultați Crearea indicatorilor pentru URL-uri și URL-uri/domenii.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="24e92-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="24e92-105">Pasul 1: Asigurați-vă de următoarele</span><span class="sxs-lookup"><span data-stu-id="24e92-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="24e92-106">Verificați dacă indicatorul este corect (fără tastare în IP/URL, acțiune corectă, grupurile RBAC corecte).</span><span class="sxs-lookup"><span data-stu-id="24e92-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="24e92-107">Așteptați minimum 2 ore după crearea indicatorului pentru a lua în considerare orice latență posibilă.</span><span class="sxs-lookup"><span data-stu-id="24e92-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="24e92-108">Confirmați că sistemele sunt instalate în Microsoft Defender pentru punct final.</span><span class="sxs-lookup"><span data-stu-id="24e92-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="24e92-109">Verificați dacă sistemele pot comunica cu cloud.</span><span class="sxs-lookup"><span data-stu-id="24e92-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="24e92-110">Verificați dacă Smartscreen este activat și accesibil, dacă ajungeți la [site-ul de test](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="24e92-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="24e92-111">Pasul 2: Depanați problema potențială</span><span class="sxs-lookup"><span data-stu-id="24e92-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="24e92-112">Asigurați-vă că clientul îndeplinește cerințele.</span><span class="sxs-lookup"><span data-stu-id="24e92-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="24e92-113">Pentru detalii, consultați [Crearea indicatorilor pentru URL-uri și URL-uri/domenii.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="24e92-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="24e92-114">Asigurați-vă că rulați cea mai recentă versiune a browserului Edge.</span><span class="sxs-lookup"><span data-stu-id="24e92-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="24e92-115">Pentru a afla cea mai recentă versiune, [consultați A afla ce versiune de Microsoft Edge aveți](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="24e92-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="24e92-116">Reporniți browserul Edge.</span><span class="sxs-lookup"><span data-stu-id="24e92-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="24e92-117">Navigați la site-ul pentru care ați configurat un indicator.</span><span class="sxs-lookup"><span data-stu-id="24e92-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="24e92-118">Dacă site-ul nu apare așa cum vă așteptați, continuați cu Pasul 3.</span><span class="sxs-lookup"><span data-stu-id="24e92-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="24e92-119">Pasul 3: Colectarea datelor</span><span class="sxs-lookup"><span data-stu-id="24e92-119">Step 3: Collect data</span></span>

- <span data-ttu-id="24e92-120">Colectați **date de diagnosticare MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="24e92-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="24e92-121">Pentru instrucțiuni, consultați [Probleme cu mașinile de bord la Microsoft Defender pentru punct final.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="24e92-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="24e92-122">Dacă sunteți confortabil să instalați și să colectați o urmărire Fiddler, consultați [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="24e92-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="24e92-123">Dacă preferați instrucțiuni de la Asistența Microsoft, selectați pictograma Asistență de mai jos pentru a deschide un caz de asistență.</span><span class="sxs-lookup"><span data-stu-id="24e92-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
