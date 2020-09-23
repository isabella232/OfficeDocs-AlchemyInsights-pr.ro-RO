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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219867"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="216a6-102">Blocarea sau deblocarea redirecționarii mesajelor de e-mail</span><span class="sxs-lookup"><span data-stu-id="216a6-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="216a6-103">Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați [Configurarea redirecționarii mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="216a6-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="216a6-104">La nivelul entității găzduite, controlul redirecționarii externe se termină utilizând politica de ieșire anti-spam.</span><span class="sxs-lookup"><span data-stu-id="216a6-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="216a6-105">Dacă este setată la dezactivat sau automat, este posibil să blocheze redirecționarea e-mailului cu eroarea "550 5.7.520 denied, organizația dumneavoastră nu permite redirecționarea externă".</span><span class="sxs-lookup"><span data-stu-id="216a6-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="216a6-106">Ulterior, dacă redirecționarea a fost setată să fie blocată, aceasta este eroarea pe care o vor vedea utilizatorii.</span><span class="sxs-lookup"><span data-stu-id="216a6-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="216a6-107">Dacă redirecționarea este blocată, asigurați-vă că politica este configurată pentru a activa autodirecționarea externă.</span><span class="sxs-lookup"><span data-stu-id="216a6-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="216a6-108">Puteți verifica Politica de filtrare antispam de ieșire din centrul de securitate și conformitate sau executând comanda Get-HostedOutboundSpamFilterPolicy | FL name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="216a6-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="216a6-109">Dacă doriți să configurați blocarea autodirecționare, aceeași comandă vă va spune acum starea de politică.</span><span class="sxs-lookup"><span data-stu-id="216a6-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="216a6-110">Notă: se recomandă să mențineți autodirecționarea externă dezactivată în politica implicită de filtrare antispam de ieșire și să o activați doar pentru utilizatorii care au nevoie de redirecționare externă, creând o politică particularizată pentru acei utilizatori.</span><span class="sxs-lookup"><span data-stu-id="216a6-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="216a6-111">Puteți citi mai multe în [Configurarea redirecționarii e-mailurilor externe în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="216a6-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>