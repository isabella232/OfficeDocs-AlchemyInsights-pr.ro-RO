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
<span data-ttu-id="12da2-p101">Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine un **Număr de cont bancar din SUA** , atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce politica DLP este în căutarea pentru atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="12da2-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="12da2-104">De exemplu, pentru o politică de **Numărul de cont bancar din SUA** cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa:</span><span class="sxs-lookup"><span data-stu-id="12da2-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="12da2-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="12da2-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="12da2-106">**[Model:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre consecutive.</span><span class="sxs-lookup"><span data-stu-id="12da2-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="12da2-107">**[Control:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici o sumă de control</span><span class="sxs-lookup"><span data-stu-id="12da2-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="12da2-108">**[Definiţie:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** O politică de DLP este încrezător că acesta a detectat acest tip de informaţii sensibile de 75 % dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="12da2-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="12da2-109">Expresie regulată Regex_usa_bank_account_number găseşte conţinut care se potriveşte cu model</span><span class="sxs-lookup"><span data-stu-id="12da2-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="12da2-110">Se găseşte un cuvânt cheie la Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="12da2-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="12da2-111">De exemplu, următoarea probă ar declanşa pentru **Numărul de cont bancar din SUA** politica: cont de verificare 78344011</span><span class="sxs-lookup"><span data-stu-id="12da2-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="12da2-112">Pentru mai multe informaţii despre ceea ce este necesar pentru un **Număr de cont bancar din SUA** să fie detectată pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri uita-te pentru numărul de cont bancar din SUA](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="12da2-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="12da2-113">Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="12da2-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

