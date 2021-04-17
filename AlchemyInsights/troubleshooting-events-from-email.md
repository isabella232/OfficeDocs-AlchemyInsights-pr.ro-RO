---
title: Depanarea evenimentelor din e-mail
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834851"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="399eb-102">Depanarea evenimentelor din e-mail</span><span class="sxs-lookup"><span data-stu-id="399eb-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="399eb-103">Verificați dacă este activată caracteristica pentru cutia poștală: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="399eb-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="399eb-104">Apoi, verificați jurnalele "Evenimente din **e-mail" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="399eb-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="399eb-105">În jurnalele "Evenimente din e-mail", găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="399eb-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="399eb-106">TrustScore determină dacă elementul este adăugat sau nu.</span><span class="sxs-lookup"><span data-stu-id="399eb-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="399eb-107">Evenimentele vor fi adăugate doar dacă TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="399eb-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="399eb-108">TrustScore este determinată de proprietățile SPF, Dkim sau Dmarc, care se află în Antetul mesajului.</span><span class="sxs-lookup"><span data-stu-id="399eb-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="399eb-109">Pentru a vizualiza aceste proprietăți:</span><span class="sxs-lookup"><span data-stu-id="399eb-109">To view these properties:</span></span>

<span data-ttu-id="399eb-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="399eb-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="399eb-111">Deschideți elementul</span><span class="sxs-lookup"><span data-stu-id="399eb-111">Open the item</span></span>
- <span data-ttu-id="399eb-112">File -> Properties -> Anteturi Internet</span><span class="sxs-lookup"><span data-stu-id="399eb-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="399eb-113">sau</span><span class="sxs-lookup"><span data-stu-id="399eb-113">or</span></span>

<span data-ttu-id="399eb-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="399eb-114">**MFCMapi**</span></span>

- <span data-ttu-id="399eb-115">Navigarea la elementul din inbox</span><span class="sxs-lookup"><span data-stu-id="399eb-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="399eb-116">Căutați un PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="399eb-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="399eb-117">Aceste proprietăți sunt determinate și înregistrate în timpul transportului și direcționării.</span><span class="sxs-lookup"><span data-stu-id="399eb-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="399eb-118">Pentru depanare suplimentară, poate fi necesar să continuați cu asistența pentru transport cu privire la erorile din SPF, DKIM și.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="399eb-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>