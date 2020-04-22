---
title: Configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645684"
---
# <a name="setup-dkim"></a>Configurare DKIM

Instrucțiunicomplete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări DKIM CNAME la serviciul de găzduire DNS al domeniului (de obicei, registratorul de domeniu). De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.

   Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:

   - **Nume gazdă**:`selector1._domainkey.<CustomDomain>`

     **Puncte de adresă sau valoare:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (

   - **Nume gazdă**:`selector2._domainkey.<CustomDomain>`

     **Puncte de adresă sau valoare:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (

   \<DomainGUID\> este textul din `.mail.protection.outlook.com` stânga înregistrării MX particularizate pentru domeniul `contoso-com` particularizat (de exemplu, pentru contoso.com de domeniu). \<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înscris la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:

   R. [conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.

   B. Selectați pictograma lansator de aplicații din stânga sus și alegeți **Admin**.

   C. În navigarea din stânga jos, extindeți **Admin** și alegeți **Exchange**.

   D. Du-te la **Protecție** > **DKIM**.

   E. Selectați domeniul, apoi **alegeți Activare** pentru **Semnare mesaje pentru acest domeniu cu semnături DKIM**. Repetați acest pas pentru fiecare domeniu particularizat.
