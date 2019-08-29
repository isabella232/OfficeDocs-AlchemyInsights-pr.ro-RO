---
title: Setup DKIM în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666276"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM în Office 365

Instrucțiunile complete pentru configurarea DKIM pentru domenii particularizate în Office 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Pentru **fiecare** domeniu particularizat, trebuie să creați **două** DKIM CNAME înregistrări la serviciul de găzduire DNS al domeniului (de obicei, Registratorul de domeniu). De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.

   Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:

   - **Nume gazdă**:`selector1._domainkey.<CustomDomain>`

     **Puncte la adresa sau valoare**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nume gazdă**:`selector2._domainkey.<CustomDomain>`

     **Puncte la adresa sau valoare**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> este textul `.mail.protection.outlook.com` din stânga în înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, `contoso-com` pentru domeniul contoso.com). \<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înscris pentru Office 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:

   R. [Conectați-vă la Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la serviciu sau de la școală.

   B. Selectați pictograma lansator de aplicații în stânga sus și alegeți **admin**.

   C. În navigare din stânga jos, extindeți **admin** și alegeți **Exchange**.

   D. Du-te la **protecția** > **DKIM**.

   E. Selectați domeniul și apoi alegeți **activați** pentru **mesaje de sign-in pentru acest domeniu cu semnături DKIM**. Repetați acest pas pentru fiecare domeniu particularizat.
