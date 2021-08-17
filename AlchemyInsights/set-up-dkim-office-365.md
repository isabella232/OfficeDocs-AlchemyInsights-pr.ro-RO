---
title: DKIM configurare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108568"
---
# <a name="setup-dkim"></a>DKIM configurare

Instrucțiunile complete pentru configurarea DKIM pentru domeniile particularizate din Microsoft 365 sunt [aici.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Pentru **fiecare** domeniu particularizat, trebuie să creați două înregistrări **DKIM** CNAME la serviciul de găzduire DNS al domeniului (de obicei, registratorul de domeniu). De exemplu, contoso.com fourthcoffee.com două înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.

   Înregistrările DKIM CNAME pentru **fiecare domeniu** particularizat utilizează următoarele formate:

   - **Nume gazdă:**`selector1._domainkey.<CustomDomain>`

     **Adresă indicati maximă sau valoare:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Nume gazdă:**`selector2._domainkey.<CustomDomain>`

     **Adresă indicati maximă sau valoare:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> este textul din partea stângă a înregistrării MX particularizate pentru domeniul particularizat `.mail.protection.outlook.com` (de exemplu, `contoso-com` pentru domeniul contoso.com). \<InitialDomain\>este domeniul pe care l-ați utilizat atunci când vă-ați Microsoft 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce ați creat înregistrările CNAME pentru domeniile dvs. particularizate, urmați următoarele instrucțiuni:

   a. [conectați-vă la Microsoft 365 cu](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) contul de la locul de muncă sau de la școală.

   b. Selectați pictograma lansator de aplicații din partea stângă sus și alegeți **Administrator**.

   c. În navigarea din stânga jos, extindeți **Admin** și **alegeți Exchange**.

   d. Accesați   >  **DKIM de protecție**.

   e. Selectați domeniul, apoi **alegeți Activare** **pentru Mesaje de semnătură pentru acest domeniu cu semnături DKIM.** Repetați acest pas pentru fiecare domeniu particularizat.
