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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994835"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurarea DKIM cu domenii particularizate

Trebuie să publicați două înregistrări CNAME pentru fiecare domeniu particularizat în DNS. Pentru a face acest lucru, utilizați următorul format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** este textul din partea stângă a **.mail.protection.outlook.com** din înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, contoso-com pentru domeniul **contoso.com**). **InitialDomain** este domeniul pe care l-ați utilizat atunci când vă ați înscris pentru Office 365 (de exemplu, **contoso.onmicrosoft.com**).

Pentru mai multe informații despre înregistrările DNS, [consultați Crearea de înregistrări DNS la orice furnizor de găzduire DNS pentru Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).