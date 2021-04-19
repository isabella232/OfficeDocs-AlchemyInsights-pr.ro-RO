---
title: Rezolvarea problemelor de autentificare SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826427"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="156e7-102">Rezolvarea problemelor de autentificare SMTP</span><span class="sxs-lookup"><span data-stu-id="156e7-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="156e7-103">Dacă primiți erorile 5.7.57 sau 5.7.3 atunci când căutați să trimiteți mesaje de e-mail SMTP și să vă autentificați cu un client sau cu o aplicație, există câteva lucruri pe care ar trebui să le verificați:</span><span class="sxs-lookup"><span data-stu-id="156e7-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="156e7-104">Remiterea SMTP autentificată poate fi dezactivată în entitatea dvs. găzduită sau în cutia poștală pe care încearcă să o utilizați (verificați ambele setări).</span><span class="sxs-lookup"><span data-stu-id="156e7-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="156e7-105">Pentru a citi mai multe, consultați [Activarea sau dezactivarea remiterii SMTP client autentificat.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="156e7-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="156e7-106">Verificați dacă [sunt activate valorile implicite de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) securitate Azure pentru entitatea dvs. găzduită; Dacă este activată, autentificarea SMTP utilizând autentificarea de bază (numită și moștenit; aceasta va utiliza numele de utilizator și parola) nu va reuși.</span><span class="sxs-lookup"><span data-stu-id="156e7-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
