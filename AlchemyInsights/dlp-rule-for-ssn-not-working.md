---
title: DLP regulă pentru SSN nu de lucru
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529878"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP probleme cu numărul de securitate socială

Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţin un **Social Security Number (SSN)** atunci când se utilizează un tip de informaţii sensibile din Office 365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce este în căutarea DLP politica. 
  
De exemplu, pentru o politică de SSN configurat cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, care poate fi într-un model formatate sau neformatate

- **[Model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru functii uite pentru SSNs în patru modele diferite:

  - Func_ssn gaseste SSNs cu pre-2011 puternic formatări care sunt formatate cu liniuţe sau spatii (val de ddd dd OR ddd dd vi)

  - Func_unformatted_ssn gaseste SSNs cu pre-2011 puternic formatări care sunt neformatat ca nouă cifre consecutive (Elena)

  - Func_randomized_formatted_ssn constată post-2011 SSNs care sunt formatate cu liniuţe sau spatii (val de ddd dd OR ddd dd vi)

  - Func_randomized_unformatted_ssn constată post-2011 SSNs care sunt neformatat ca nouă cifre consecutive (Elena)

- **[Control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nu, nu există nici o sumă de control

- **[Definiţie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** O politică de DLP este 85 % încrezător că a detectat acest tip de informaţii sensibile dacă, într-o proximitate de 300 de caractere:

  - [Funcţia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) găseşte conţinut care se potriveşte model.

  - Se găseşte un cuvânt cheie la [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Exemple de cuvinte cheie include: *securitate socială, securitate socială #, Soc Sec, SSN* . De exemplu, următoarea probă ar declanşa pentru politica DLP SSN: **SSN: 489-36-8350**
  
Pentru mai multe informaţii despre ceea ce este necesar pentru SSNs să fie detectate pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri uite pentru SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  