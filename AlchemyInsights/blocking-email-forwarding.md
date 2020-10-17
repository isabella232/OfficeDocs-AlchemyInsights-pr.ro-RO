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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473113"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocarea sau deblocarea redirecționarii mesajelor de e-mail

Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați [Configurarea redirecționarii mesajelor de e-mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

La nivelul entității găzduite, controlul redirecționarii externe se termină utilizând politica de spam de ieșire. Puteți verifica Politica de filtrare antispam de ieșire din centrul de securitate și conformitate [aici] ( https://protection.office.com/antispam) sau utilizând [comanda Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Dacă primiți următoarea eroare: **"550 5.7.520 Access Denied, organizația dumneavoastră nu permite redirecționarea externă"**, asigurați-vă că politica este configurată pentru a activa redirecționarea automată externă.

**Notă:** Se recomandă să mențineți autodirecționarea externă dezactivată în politica implicită de filtrare antispam de ieșire și să o activați doar pentru utilizatorii care au nevoie de redirecționare externă, creând o politică particularizată pentru acei utilizatori. Puteți citi mai multe în [Configurarea redirecționarii e-mailurilor externe în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).