---
title: DLP regulă pentru noi numărul de cont bancar nu de lucru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29484902"
---
Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine un **Număr de cont bancar din SUA** , atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce politica DLP este în căutarea pentru atunci când este evaluată. 
  
De exemplu, pentru o politică de **Numărul de cont bancar din SUA** cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa: 
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre 
    
- **[Model:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre consecutive. 
    
- **[Control:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici o sumă de control 
    
- **[Definiţie:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** O politică de DLP este încrezător că acesta a detectat acest tip de informaţii sensibile de 75 % dacă, într-o proximitate de 300 de caractere: 
    
  - Expresie regulată Regex_usa_bank_account_number găseşte conţinut care se potriveşte cu model
    
  - Se găseşte un cuvânt cheie la Keyword_usa_Bank_Account.
    
    De exemplu, următoarea probă ar declanşa pentru **Numărul de cont bancar din SUA** politica: cont de verificare 78344011 
    
Pentru mai multe informaţii despre ceea ce este necesar pentru un **Număr de cont bancar din SUA** să fie detectată pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri uita-te pentru numărul de cont bancar din SUA](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

