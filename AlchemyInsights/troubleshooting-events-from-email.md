---
title: Depanarea evenimentelor din E-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658746"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="a233e-102">Depanarea evenimentelor din E-mail</span><span class="sxs-lookup"><span data-stu-id="a233e-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="a233e-103">Verificați dacă este activată caracteristica pentru cutia poștală: **Get-EventsFromEmailConfiguration <mailbox> -Identity**</span><span class="sxs-lookup"><span data-stu-id="a233e-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="a233e-104">Apoi, uitați-vă la "evenimente din e-mailul" jurnalele de **Export-MailboxDiagnosticLogs <mailbox> -componenta TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="a233e-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="a233e-105">În jurnalele "evenimente din E-mail", găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="a233e-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="a233e-106">TrustScore determină dacă elementul este adăugat sau nu.</span><span class="sxs-lookup"><span data-stu-id="a233e-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="a233e-107">Evenimentele vor fi adăugate doar dacă TrustScore = "de încredere".</span><span class="sxs-lookup"><span data-stu-id="a233e-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="a233e-108">TrustScore este determinată de proprietățile SPF, DKIM sau DMARC, care se află în antetul mesajului.</span><span class="sxs-lookup"><span data-stu-id="a233e-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="a233e-109">Pentru a vizualiza aceste proprietăți:</span><span class="sxs-lookup"><span data-stu-id="a233e-109">To view these properties:</span></span>

<span data-ttu-id="a233e-110">**Outlook pentru desktop**</span><span class="sxs-lookup"><span data-stu-id="a233e-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="a233e-111">Deschiderea elementului</span><span class="sxs-lookup"><span data-stu-id="a233e-111">Open the item</span></span>
- <span data-ttu-id="a233e-112">Fișier-> proprietăți-> anteturi de Internet</span><span class="sxs-lookup"><span data-stu-id="a233e-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="a233e-113">sau</span><span class="sxs-lookup"><span data-stu-id="a233e-113">or</span></span>

<span data-ttu-id="a233e-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="a233e-114">**MFCMapi**</span></span>

- <span data-ttu-id="a233e-115">Navigarea la elementul din Inbox</span><span class="sxs-lookup"><span data-stu-id="a233e-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="a233e-116">Căutați PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="a233e-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="a233e-117">Aceste proprietăți sunt determinate și înregistrate în timpul transportului și rutare.</span><span class="sxs-lookup"><span data-stu-id="a233e-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="a233e-118">Pentru depanarea ulterioară, poate fi necesar să urmăriți asistența pentru transport cu privire la erorile din SPF, DKIM și. or DMARC.</span><span class="sxs-lookup"><span data-stu-id="a233e-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>