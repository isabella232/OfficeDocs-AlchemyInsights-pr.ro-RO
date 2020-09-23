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
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocarea sau deblocarea redirecționarii mesajelor de e-mail

Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați [Configurarea redirecționarii mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

La nivelul entității găzduite, controlul redirecționarii externe se termină utilizând politica de ieșire anti-spam. Dacă este setată la dezactivat sau automat, este posibil să blocheze redirecționarea e-mailului cu eroarea "550 5.7.520 denied, organizația dumneavoastră nu permite redirecționarea externă". Ulterior, dacă redirecționarea a fost setată să fie blocată, aceasta este eroarea pe care o vor vedea utilizatorii.

Dacă redirecționarea este blocată, asigurați-vă că politica este configurată pentru a activa autodirecționarea externă. Puteți verifica Politica de filtrare antispam de ieșire din centrul de securitate și conformitate sau executând comanda Get-HostedOutboundSpamFilterPolicy | FL name, AutoForwardingMode. Dacă doriți să configurați blocarea autodirecționare, aceeași comandă vă va spune acum starea de politică.

Notă: se recomandă să mențineți autodirecționarea externă dezactivată în politica implicită de filtrare antispam de ieșire și să o activați doar pentru utilizatorii care au nevoie de redirecționare externă, creând o politică particularizată pentru acei utilizatori. Puteți citi mai multe în [Configurarea redirecționarii e-mailurilor externe în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).