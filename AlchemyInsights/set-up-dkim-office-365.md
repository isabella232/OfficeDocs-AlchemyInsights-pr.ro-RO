---
title: DKIM de configurare
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808719"
---
# <a name="setup-dkim"></a>DKIM de configurare

Instrucțiunile complete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări CNAME DKIM la serviciul de găzduire DNS al domeniului (de obicei, Registratorul de domeniu). De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări CNAME DKIM: două pentru contoso.com și două pentru fourthcoffee.com.

   Înregistrările CNAME DKIM pentru **fiecare** domeniu particularizat utilizează următoarele formate:

   - **Nume gazdă**: `selector1._domainkey.<CustomDomain>`

     **Indică adresa sau valoarea**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nume gazdă**: `selector2._domainkey.<CustomDomain>`

     **Indică adresa sau valoarea**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> este textul de la stânga `.mail.protection.outlook.com` în înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, `contoso-com` pentru domeniul contoso.com). \<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înregistrat la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce ați creat înregistrările CNAME pentru domeniile particularizate, parcurgeți următoarele instrucțiuni:

   un. [Conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.

   b. Selectați pictograma lansator de aplicații din partea stângă sus și alegeți **administrator**.

   c. În navigarea din stânga jos, extindeți **administratorul** și alegeți **Exchange**.

   d. Accesați DKIM de **protecție**  >  **DKIM**.

   e. Selectați domeniul, apoi alegeți **Activare** pentru **semnați mesaje pentru acest domeniu cu semnături DKIM**. Repetați acest pas pentru fiecare domeniu particularizat.
