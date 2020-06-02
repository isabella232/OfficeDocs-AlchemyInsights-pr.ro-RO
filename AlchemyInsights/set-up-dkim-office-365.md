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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509396"
---
# <a name="setup-dkim"></a>Configurare DKIM

Instrucțiunicomplete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări DKIM CNAME la serviciul de găzduire DNS al domeniului (de obicei, registratorul de domeniu). De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.

   Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:

   - **Nume gazdă**:`selector1._domainkey.<CustomDomain>`

     **Puncte de adresă sau valoare:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (

   - **Nume gazdă**:`selector2._domainkey.<CustomDomain>`

     **Puncte de adresă sau valoare:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600 (

   \<DomainGUID\>este textul din stânga `.mail.protection.outlook.com` înregistrării MX particularizate pentru domeniul particularizat (de exemplu, `contoso-com` pentru contoso.com de domeniu). \<InitialDomain\>este domeniul pe care l-ați utilizat atunci când v-ați înscris la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:

   R. [conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.

   B. Selectați pictograma lansator de aplicații din stânga sus și alegeți **Admin**.

   C. În navigarea din stânga jos, extindeți **Admin** și alegeți **Exchange**.

   D. Du-te la **Protecție**  >  **DKIM**.

   E. Selectați domeniul, apoi **alegeți Activare** pentru **Semnare mesaje pentru acest domeniu cu semnături DKIM**. Repetați acest pas pentru fiecare domeniu particularizat.
