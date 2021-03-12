---
title: Configurarea DKIM cu domenii particularizate
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747639"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurarea DKIM cu domenii particularizate

Trebuie să publicați două înregistrări CNAME pentru fiecare domeniu particularizat din DNS. Pentru a face acest lucru, utilizați următorul format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** este textul de la stânga **. mail.Protection.Outlook.com** în înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, contoso-com pentru domeniul **contoso.com**). **InitialDomain** este domeniul pe care l-ați utilizat atunci când v-ați înregistrat la Office 365 (de exemplu, **contoso.onmicrosoft.com**).

Pentru mai multe informații despre înregistrările DNS, consultați [crearea de înregistrări DNS la orice furnizor de găzduire DNS pentru Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).