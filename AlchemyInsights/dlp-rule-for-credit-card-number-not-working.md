---
title: DLP regulă pentru numărul cardului de Credit nu de lucru
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529967"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleme cu numere de Card de Credit

Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine un **Număr de Card de Credit** , atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru a declanşa politica DLP atunci când este evaluată. De exemplu, pentru un **Card de Credit politica** configurat cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddd) şi trebuie să treacă testul Luhn.

- **[Model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Model foarte complexă şi robustă care detectează cardurile de la toate marile branduri din întreaga lume, inclusiv Visa, MasterCard, descopera carte, JCB, American Express, carduri cadou, şi carduri de cina.

- **[Control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, control Luhn

- **[Definiţie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** O politică de DLP este 85 % încrezător că a detectat acest tip de informaţii sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcţia Func_credit_card găseşte conţinut care se potriveşte model.

  - Este adevărată una dintre următoarele:

  - Se găseşte un cuvânt cheie la Keyword_cc_verification.

  - Se găseşte un cuvânt cheie la Keyword_cc_name

  - Funcţia Func_expiration_date constată o dată în formatul corect.

  - Control trece

    De exemplu, următoarea probă ar declanşa pentru o politică de număr de Card de Credit DLP:

  - Viza: 4485 3647 3952 7352
  
  - Expira: 2/2009

Pentru mai multe informaţii despre ceea ce este necesar pentru un **Număr de Card de Credit** să fie detectată pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri arata pentru cardul de Credit #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  