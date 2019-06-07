---
title: Configurare DKIM în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765341"
---
# <a name="setup-dkim-in-office-365"></a>Configurare DKIM în Office 365

Instrucţiuni complete pentru configurarea DKIM pentru domenii particularizate în Office 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Pentru **fiecare** domeniu personalizat, trebuie să creaţi **două** înregistrări DKIM CNAME la serviciul găzduire DNS al domeniului (de obicei, Registratorul de domeniu). De exemplu, contoso.com şi fourthcoffee.com necesită patru DKIM CNAME records: două pentru contoso.com şi două pentru fourthcoffee.com.

   Înregistrările DKIM CNAME pentru **fiecare** domeniu personalizat utilizează următoarele formate:

   - **Nume gazdă**:`selector1._domainkey.<CustomDomain>`

     **Puncte la adresa sau valoare**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Nume gazdă**:`selector2._domainkey.<CustomDomain>`

     **Puncte la adresa sau valoare**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> este textul din stanga `.mail.protection.outlook.com` în personalizate înregistrarea MX pentru domeniul personalizate (de exemplu, `contoso-com` pentru domeniul contoso.com). \<InitialDomain\> este un domeniu de aţi folosit atunci când v-aţi înscris pentru Office 365 (de exemplu, contoso.onmicrosoft.com).

2. După ce aţi creat înregistrări CNAME pentru domenii particularizate, completaţi următoarele instrucţiuni:

   un. [Conectaţi-vă la Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul dvs de lucru sau şcoală.

   b. Selectaţi pictograma app lansator din stânga şi selectaţi **Admin**.

   c. În stânga de navigare, extindeţi **Admin** şi alege **Exchange**.

   d. Du-te la **protectia** > **DKIM**.

   e. Selectaţi domeniul şi apoi **permite** pentru **semn mesaje pentru acest domeniu, cu semnăturile de DKIM**. Repetaţi acest pas pentru fiecare domeniu particularizat.
