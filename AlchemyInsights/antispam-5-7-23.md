---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682256"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="6fc7d-102">Fix probleme de livrare e-mail pentru codul de eroare 5.7.23</span><span class="sxs-lookup"><span data-stu-id="6fc7d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="6fc7d-103">Verificați înregistrarea SPF DNS pentru domeniu la un verificator de înregistrări SPF sau DNS disponibile public pe web.</span><span class="sxs-lookup"><span data-stu-id="6fc7d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="6fc7d-104">Verificați că mesajul de ieșire nu a fost identificat ca spam de Office 365 și rutate prin [rezervorul de livrare de risc ridicat](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="6fc7d-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="6fc7d-105">Mesajele din rezervorul de livrare cu risc ridicat nu vor trece de controalele SPF și, prin urmare, nu vor fi acceptate de organizația de e-mail de destinație.</span><span class="sxs-lookup"><span data-stu-id="6fc7d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="6fc7d-106">Dacă problema persistă, poate fi necesar să contactați administratorul gazdă de poștă electronică la care încercați să trimiteți e-mailuri.</span><span class="sxs-lookup"><span data-stu-id="6fc7d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="6fc7d-107">Notați eroarea externă detaliată disponibilă în mesajul de respingere.</span><span class="sxs-lookup"><span data-stu-id="6fc7d-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="6fc7d-108">Este posibil ca asistența Office 365 să nu poată asista în continuare.</span><span class="sxs-lookup"><span data-stu-id="6fc7d-108">Office 365 support may not be able to assist further.</span></span>