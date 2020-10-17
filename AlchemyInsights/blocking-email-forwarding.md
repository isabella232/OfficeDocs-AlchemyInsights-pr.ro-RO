---
title: 726 blocarea redirecționarii mesajelor de e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478317"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="12145-102">Blocarea sau deblocarea redirecționarii mesajelor de e-mail</span><span class="sxs-lookup"><span data-stu-id="12145-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="12145-103">Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați [Configurarea redirecționarii mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="12145-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="12145-104">La nivelul entității găzduite, controlul redirecționarii externe se termină utilizând politica de spam de ieșire.</span><span class="sxs-lookup"><span data-stu-id="12145-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="12145-105">Puteți să verificați politica de filtrare antispam de ieșire din centrul de securitate și conformitate [aici](https://protection.office.com/antispam) sau utilizând [comanda Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="12145-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="12145-106">Dacă primiți următoarea eroare: **"550 5.7.520 Access Denied, organizația dumneavoastră nu permite redirecționarea externă"**, asigurați-vă că politica este configurată pentru a activa redirecționarea automată externă.</span><span class="sxs-lookup"><span data-stu-id="12145-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="12145-107">**Notă:** Se recomandă să mențineți autodirecționarea externă dezactivată în politica implicită de filtrare antispam de ieșire și să o activați doar pentru utilizatorii care au nevoie de redirecționare externă, creând o politică particularizată pentru acei utilizatori.</span><span class="sxs-lookup"><span data-stu-id="12145-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="12145-108">Puteți citi mai multe în [Configurarea redirecționarii e-mailurilor externe în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="12145-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>