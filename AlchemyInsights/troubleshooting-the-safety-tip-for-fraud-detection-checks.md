---
title: Vârful de siguranţă pentru detectarea fraudei de depanare verifică
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353261"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c53e7-102">Vârful de siguranţă pentru detectarea fraudei de depanare verifică</span><span class="sxs-lookup"><span data-stu-id="c53e7-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c53e7-103">Dacă sunteţi Noţiuni de bază un sfat de siguranţă care spune "expeditorul nu a reuşit noastre controale de detectare fraude şi nu poate fi care apar a fi", apoi expeditorul nu a reuşit să treacă DKIM fie SPF verificări de autentificare.</span><span class="sxs-lookup"><span data-stu-id="c53e7-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c53e7-104">Cea mai bună metodă pentru a rezolva acest lucru este pentru expeditorului să autorizeze ei înşişi.</span><span class="sxs-lookup"><span data-stu-id="c53e7-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c53e7-105">Dacă expeditorul este de a trimite în numele dumneavoastră, trebuie să le autorizeze prin adăugarea adresa de IP a expeditorului la SPF record.</span><span class="sxs-lookup"><span data-stu-id="c53e7-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c53e7-106">Vedeți [Depanarea vârful roşu de siguranţă (suspect) pentru detectarea fraudei controale](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="c53e7-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c53e7-107">Aici sunt câteva alte link-uri care vă pot ajuta:</span><span class="sxs-lookup"><span data-stu-id="c53e7-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c53e7-108">Cum Office 365 utilizează expeditor politică framework (SPF) pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="c53e7-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c53e7-109">Înfiinţat SPF în Office 365 pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="c53e7-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
