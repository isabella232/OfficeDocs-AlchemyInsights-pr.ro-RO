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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332319"
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
**Notă:** **DomainGUID** este textul din partea stângă a **.mail.protection.outlook.com** din înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, contoso-com pentru domeniul **contoso.com**). **InitialDomain este** domeniul pe care l-ați utilizat atunci când vă-ați înscris pentru Office 365 (de exemplu, **contoso.onmicrosoft.com**).

Pentru mai multe informații despre înregistrările DNS, [consultați Crearea de înregistrări DNS la orice furnizor de găzduire DNS pentru Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).