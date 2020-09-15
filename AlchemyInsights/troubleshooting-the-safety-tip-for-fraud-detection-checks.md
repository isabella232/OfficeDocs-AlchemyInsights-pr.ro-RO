---
title: Depanarea Sfatului de siguranță pentru controalele de detectare a fraudei
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658422"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="9b3c6-102">Depanarea Sfatului de siguranță pentru controalele de detectare a fraudei</span><span class="sxs-lookup"><span data-stu-id="9b3c6-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="9b3c6-103">Dacă primiți un sfat de siguranță care spune "expeditorul nu a reușit să verifice controalele de detectare a fraudei și poate să nu fie cine se pare", atunci expeditorul nu a reușit să treacă de controalele de autentificare DKIM sau SPF.</span><span class="sxs-lookup"><span data-stu-id="9b3c6-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="9b3c6-104">Cea mai bună metodă de a rezolva acest lucru este ca expeditorul să se autorizeze.</span><span class="sxs-lookup"><span data-stu-id="9b3c6-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="9b3c6-105">Dacă expeditorul trimite în numele dvs., trebuie să-i autorizați prin adăugarea adresei IP a expeditorului în înregistrarea SPF.</span><span class="sxs-lookup"><span data-stu-id="9b3c6-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="9b3c6-106">Consultați [Depanarea vârfului de siguranță roșu (suspicios) pentru controalele de detectare a fraudelor](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="9b3c6-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="9b3c6-107">Iată alte câteva linkuri care vă pot ajuta:</span><span class="sxs-lookup"><span data-stu-id="9b3c6-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="9b3c6-108">Cum utilizează Microsoft Framework Policy (SPF) pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="9b3c6-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="9b3c6-109">Configurați SPF pentru a preveni falsificarea</span><span class="sxs-lookup"><span data-stu-id="9b3c6-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
