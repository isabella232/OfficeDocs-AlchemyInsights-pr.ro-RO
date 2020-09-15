---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717337"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="2fae7-102">Remedierea problemelor de livrare a mesajelor de e-mail pentru codul de eroare 5.7.23</span><span class="sxs-lookup"><span data-stu-id="2fae7-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="2fae7-103">Verificați înregistrarea SPF DNS pentru domeniul dvs., într-un verificator de înregistrare SPF sau DNS, disponibil public pe web.</span><span class="sxs-lookup"><span data-stu-id="2fae7-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="2fae7-104">Verificați dacă mesajul de ieșire nu a fost identificat ca spam de către Microsoft și a fost distribuit prin [bazinul cu risc ridicat](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="2fae7-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="2fae7-105">Mesajele din bazinul de livrare cu risc ridicat nu vor trece de controalele SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.</span><span class="sxs-lookup"><span data-stu-id="2fae7-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="2fae7-106">Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți mesaje de e-mail.</span><span class="sxs-lookup"><span data-stu-id="2fae7-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="2fae7-107">Notați eroarea externă detaliată disponibilă în mesajul Bounce.</span><span class="sxs-lookup"><span data-stu-id="2fae7-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="2fae7-108">Asistența Microsoft poate să nu mai poată ajuta în continuare.</span><span class="sxs-lookup"><span data-stu-id="2fae7-108">Microsoft support may not be able to assist further.</span></span>
