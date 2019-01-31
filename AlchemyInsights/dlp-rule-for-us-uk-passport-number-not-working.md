---
title: DLP regulă pentru US / UK numărul pașaportului neactiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656435"
---
<span data-ttu-id="1b3e9-p101">Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine o **U.S. / numărul de paşaport UK** atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce politica DLP este în căutarea pentru atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="1b3e9-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="1b3e9-104">De exemplu, pentru o **U.S. / numărul de paşaport UK** politica configurat cu un nivel de încredere de 75 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa</span><span class="sxs-lookup"><span data-stu-id="1b3e9-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="1b3e9-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nouă cifre</span><span class="sxs-lookup"><span data-stu-id="1b3e9-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="1b3e9-106">**[Model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nouă cifre consecutive</span><span class="sxs-lookup"><span data-stu-id="1b3e9-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="1b3e9-107">**[Control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici o sumă de control</span><span class="sxs-lookup"><span data-stu-id="1b3e9-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="1b3e9-108">**[Definiţie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** O politică de DLP este încrezător că acesta a detectat acest tip de informaţii sensibile de 75 % dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="1b3e9-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="1b3e9-109">Funcţia Func_usa_uk_passport găseşte conţinut care se potriveşte model.</span><span class="sxs-lookup"><span data-stu-id="1b3e9-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="1b3e9-110">Se găseşte un cuvânt cheie la Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="1b3e9-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="1b3e9-111">De exemplu, următoarea probă ar declanşa pentru **U.S. / numărul de paşaport UK** politica: numărul de paşaport SUA 123456789</span><span class="sxs-lookup"><span data-stu-id="1b3e9-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="1b3e9-112">Pentru mai multe informaţii despre ceea ce este necesar pentru o nouă / UK numărul paşaportului pentru a fi detectate pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Uite ce Sensitive informaţii tipuri pentru SUA / Marea Britanie pașaport numărul](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="1b3e9-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="1b3e9-113">Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1b3e9-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

