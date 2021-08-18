---
title: Blocarea sau deblocarea redirecționării automate externe a e-mailului
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897480"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blocarea sau deblocarea redirecționării automate a e-mailurilor

Pentru a activa sau a dezactiva redirecționarea e-mailului pentru o anumită cutie poștală, consultați Configurarea [redirecționării e-mailului.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administratorii pot controla redirecționarea externă pentru organizație, utilizând [politicile de spam de ieșire.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Gestionați politicile pentru spam de ieșire în portalul Microsoft 365 Defender la sau utilizând <https://security.microsoft.com/antispam> cmdletul [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) în Exchange Online PowerShell.

Dacă primiți următoarea eroare: **"550 5.7.520 Acces refuzat,** Organizația dvs. nu permite redirecționarea externă", asigurați-vă că politica este configurată pentru a activa mesajele externe redirecționate automat.

**Notă:** Am recomandat valoarea implicită Automat  **-** Sistem controlat pentru setarea Reguli de redirecționare automată din politica implicită de filtrare antispam de ieșire (redirecționarea externă automată este blocată; redirecționarea automată internă funcționează în continuare). Ar trebui să creați politici personalizate de filtrare antispam de ieșire și să utilizați valoarea Activat **-** Redirecționarea este activată doar pentru utilizatorii care au nevoie de redirecționarea automată a e-mailurilor externe. Pentru mai multe informații, consultați Configurarea [redirecționării e-mailului extern în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
