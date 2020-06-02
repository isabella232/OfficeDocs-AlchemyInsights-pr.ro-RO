---
title: Depanarea bacșișului de siguranță pentru verificările de detectare a fraudelor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504995"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="bc9b1-102">Depanarea bacșișului de siguranță pentru verificările de detectare a fraudelor</span><span class="sxs-lookup"><span data-stu-id="bc9b1-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="bc9b1-103">Dacă primiți un sfat de siguranță care spune "Expeditorul nu a reușit verificările noastre de detectare a fraudei și nu poate fi cine par a fi", atunci expeditorul nu a reușit să treacă fie DKIM sau SPF controale de autentificare.</span><span class="sxs-lookup"><span data-stu-id="bc9b1-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="bc9b1-104">Cea mai bună metodă pentru a rezolva acest lucru este pentru expeditor să se autorizeze.</span><span class="sxs-lookup"><span data-stu-id="bc9b1-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="bc9b1-105">Dacă expeditorul trimite în numele dvs., trebuie să-i autorizați adăugând adresa IP a expeditorului la înregistrarea SPF.</span><span class="sxs-lookup"><span data-stu-id="bc9b1-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="bc9b1-106">Consultați [Depanarea vârfului roșu (suspect) de siguranță pentru verificările de detectare a fraudei](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="bc9b1-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="bc9b1-107">Iată alte câteva link-uri care pot ajuta:</span><span class="sxs-lookup"><span data-stu-id="bc9b1-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="bc9b1-108">utilizează Microsoft cadrul de politică expeditor (SPF) pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="bc9b1-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="bc9b1-109">Configurarea SPF pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="bc9b1-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
