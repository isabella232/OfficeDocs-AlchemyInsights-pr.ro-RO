---
title: 726 Blocarea redirecționării e-mailului
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059644"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocarea sau deblocarea redirecționării e-mailului

Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați Configurarea [redirecționării e-mailului.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

La nivel de entitate găzduită, controlul redirecționării externe se face utilizând politica de spam de ieșire. Puteți verifica politica de filtrare antispam [](https://protection.office.com/antispam) de ieșire din Centrul de securitate și conformitate aici sau utilizând comanda [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Dacă primiți următoarea eroare: **"550 5.7.520 Acces refuzat,** Organizația dvs. nu permite redirecționarea externă", asigurați-vă că politica este configurată pentru a activa Redirecționarea automată externă.

**Notă:** Se recomandă să mențineți avansarea externă dezactivată în politica implicită de filtrare antispam de ieșire și să o activați doar pentru utilizatorii care au nevoie de redirecționare externă, creând o politică personalizată pentru acei utilizatori. Puteți citi mai multe în Configurarea [redirecționării e-mailului extern în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).