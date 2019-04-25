---
title: DLP regulă pentru US / UK numărul pașaportului neactiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404393"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme cu DLP - U.S. / numere de paşaport din Marea Britanie

Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine o **U.S. / numărul de paşaport UK** atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce politica DLP este în căutarea pentru atunci când este evaluată. 
  
De exemplu, pentru o **U.S. / numărul de paşaport UK** politica configurat cu un nivel de încredere de 75 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nouă cifre 
    
- **[Model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nouă cifre consecutive 
    
- **[Control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici o sumă de control 
    
- **[Definiţie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** O politică de DLP este încrezător că acesta a detectat acest tip de informaţii sensibile de 75 % dacă, într-o proximitate de 300 de caractere: 
    
  - Funcţia Func_usa_uk_passport găseşte conţinut care se potriveşte model.
    
  - Se găseşte un cuvânt cheie la Keyword_passport.
    
    De exemplu, următoarea probă ar declanşa pentru **U.S. / numărul de paşaport UK** politica: numărul de paşaport SUA 123456789 
    
Pentru mai multe informaţii despre ceea ce este necesar pentru o nouă / UK numărul paşaportului pentru a fi detectate pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Uite ce Sensitive informaţii tipuri pentru SUA / Marea Britanie pașaport numărul](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

