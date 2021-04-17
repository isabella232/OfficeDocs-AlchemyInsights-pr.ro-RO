---
title: Depanarea sfaturilor de siguranță pentru detectarea fraudelor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834743"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="eaf2f-102">Depanarea sfaturilor de siguranță pentru detectarea fraudelor</span><span class="sxs-lookup"><span data-stu-id="eaf2f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="eaf2f-103">Dacă obțineți un sfat de siguranță care spune "Expeditorul nu a reușit verificările de detectare a fraudelor și este posibil să nu fie cine pare să fie", expeditorul nu a trecut nici verificările de autentificare DKIM, nici SPF.</span><span class="sxs-lookup"><span data-stu-id="eaf2f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="eaf2f-104">Cea mai bună metodă de a rezolva această problemă este ca expeditorul să se autorizeze singur.</span><span class="sxs-lookup"><span data-stu-id="eaf2f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="eaf2f-105">Dacă expeditorul trimite în numele dvs., trebuie să îl autorizați adăugând adresa IP a expeditorului la înregistrarea SPF.</span><span class="sxs-lookup"><span data-stu-id="eaf2f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="eaf2f-106">Consultați [Depanarea sfatului de siguranță roșu (suspect) pentru detectarea fraudelor și a verificărilor](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="eaf2f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="eaf2f-107">Iată alte câteva linkuri care vă pot ajuta:</span><span class="sxs-lookup"><span data-stu-id="eaf2f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="eaf2f-108">Cum utilizează Microsoft sender Policy Framework (SPF) pentru a preveni falsofingul</span><span class="sxs-lookup"><span data-stu-id="eaf2f-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="eaf2f-109">Configurați SPF pentru a contribui la prevenirea falsării</span><span class="sxs-lookup"><span data-stu-id="eaf2f-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
