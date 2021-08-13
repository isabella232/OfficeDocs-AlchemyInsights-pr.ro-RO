---
title: Utilizarea site-ului web Wix Office 365 domenii achiziționate sau gestionate
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
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980189"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utilizarea site-ului web Wix Office 365 domenii achiziționate sau gestionate

- [Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Articolul Wix "Conectarea unui domeniu la Wix utilizând metoda de indicație" recomandă să utilizați indicația (adăugarea de înregistrări DNS conform linkului de mai sus), în loc să modificați serverele de nume atunci când utilizați Office 365
- Dacă alegeți în continuare să modificați serverele de nume la Wix, va trebui  [să creați înregistrări DNS la Wix pentru Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Dacă domeniul a fost achiziționat de la Microsoft, serverele de nume nu pot fi modificate. Dacă trebuie să schimbați numele serverelor, domeniul achiziționat de Microsoft va trebui să fie transferat la alt furnizor  [de găzduire după 60 de zile](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)