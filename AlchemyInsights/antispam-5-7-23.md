---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506455"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="35fa2-102">Remediați problemele de livrare de e-mail pentru codul de eroare 5.7.23</span><span class="sxs-lookup"><span data-stu-id="35fa2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="35fa2-103">Verificați înregistrarea SPF DNS pentru domeniul dvs., la un verificatorul de înregistrări SPF sau DNS disponibil publicului pe web.</span><span class="sxs-lookup"><span data-stu-id="35fa2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="35fa2-104">Verificați dacă mesajul de ieșire nu a fost identificat ca spam de microsoft și distribuit prin [rezervorul de livrare cu risc ridicat](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="35fa2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="35fa2-105">Mesajele din rezervorul de livrare cu risc ridicat nu vor trece de verificările SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.</span><span class="sxs-lookup"><span data-stu-id="35fa2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="35fa2-106">Dacă problema persistă, poate fi necesar să contactați administratorul gazdei de e-mail la care încercați să trimiteți e-mailuri.</span><span class="sxs-lookup"><span data-stu-id="35fa2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="35fa2-107">Notați eroarea externă detaliată disponibilă în mesajul de respingere.</span><span class="sxs-lookup"><span data-stu-id="35fa2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="35fa2-108">Este posibil ca asistența Microsoft să nu poată fi asistată în continuare.</span><span class="sxs-lookup"><span data-stu-id="35fa2-108">Microsoft support may not be able to assist further.</span></span>
