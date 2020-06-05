---
title: Depanarea evenimentelor din e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569406"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="8eeea-102">Depanarea evenimentelor din e-mail</span><span class="sxs-lookup"><span data-stu-id="8eeea-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="8eeea-103">Verificați caracteristica este activată pentru cutia poștală: \*\*Get-EventsFromEmailConfiguration -Identitate <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="8eeea-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="8eeea-104">Apoi, uita-te la "Evenimente din e-mail" jurnalele **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="8eeea-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="8eeea-105">În jurnalele 'Evenimente din e-mail', găsiți InternetMessageId care se potrivește cu elementul din cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="8eeea-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="8eeea-106">Scorul de încredere determină dacă elementul este adăugat sau nu.</span><span class="sxs-lookup"><span data-stu-id="8eeea-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="8eeea-107">Evenimentele vor fi adăugate numai dacă TrustScore = "Încredere".</span><span class="sxs-lookup"><span data-stu-id="8eeea-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="8eeea-108">TrustScore este determinată de proprietățile SPF, Dkim sau Dmarc, care se află în antetul mesajului.</span><span class="sxs-lookup"><span data-stu-id="8eeea-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="8eeea-109">Pentru a vizualiza aceste proprietăți:</span><span class="sxs-lookup"><span data-stu-id="8eeea-109">To view these properties:</span></span>

<span data-ttu-id="8eeea-110">**Discutii pe forum Windows 7**</span><span class="sxs-lookup"><span data-stu-id="8eeea-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="8eeea-111">Deschiderea elementului</span><span class="sxs-lookup"><span data-stu-id="8eeea-111">Open the item</span></span>
- <span data-ttu-id="8eeea-112">Fișier -> Proprietăți -> anteturi Internet</span><span class="sxs-lookup"><span data-stu-id="8eeea-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="8eeea-113">Sau</span><span class="sxs-lookup"><span data-stu-id="8eeea-113">or</span></span>

<span data-ttu-id="8eeea-114">**Mfcmapi**</span><span class="sxs-lookup"><span data-stu-id="8eeea-114">**MFCMapi**</span></span>

- <span data-ttu-id="8eeea-115">Navigarea la elementul din inbox</span><span class="sxs-lookup"><span data-stu-id="8eeea-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="8eeea-116">Caută PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="8eeea-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="8eeea-117">Aceste proprietăți sunt determinate și înregistrate în timpul transportului și dirijării.</span><span class="sxs-lookup"><span data-stu-id="8eeea-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="8eeea-118">Pentru depanare suplimentară, poate fi necesar să urmăriți cu Asistență pentru transport despre defecțiunile din SPF, DKIM și.sau DMARC.</span><span class="sxs-lookup"><span data-stu-id="8eeea-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>