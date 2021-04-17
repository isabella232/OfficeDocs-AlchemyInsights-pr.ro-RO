---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821423"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="a19cf-102">Remediați problemele de livrare a mesajelor de e-mail pentru codul de eroare 5.7.23</span><span class="sxs-lookup"><span data-stu-id="a19cf-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="a19cf-103">Verificați înregistrarea DNS SPF pentru domeniul dvs. la un verificator de înregistrări SPF sau DNS disponibil public pe web.</span><span class="sxs-lookup"><span data-stu-id="a19cf-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="a19cf-104">Verificați dacă mesajul de ieșire nu a fost identificat ca spam de către Microsoft și distribuit prin intermediul [rezervorului de livrare pentru risc înalt.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="a19cf-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="a19cf-105">Mesajele din rezervor de livrare cu risc înalt nu vor trece verificările SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.</span><span class="sxs-lookup"><span data-stu-id="a19cf-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="a19cf-106">Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți e-mail.</span><span class="sxs-lookup"><span data-stu-id="a19cf-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="a19cf-107">Rețineți eroarea externă detaliată disponibilă în mesajul returnat.</span><span class="sxs-lookup"><span data-stu-id="a19cf-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="a19cf-108">Asistența Microsoft ar putea să nu vă mai poată ajuta.</span><span class="sxs-lookup"><span data-stu-id="a19cf-108">Microsoft support may not be able to assist further.</span></span>
