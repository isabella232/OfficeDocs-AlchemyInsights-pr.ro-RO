---
title: DLP regulă pentru numărul cardului de Credit nu de lucru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485763"
---
<span data-ttu-id="a5a0e-p101">Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţine un **Număr de Card de Credit** , atunci când se utilizează un tip de informaţii sensibile DLP în O365? Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru a declanşa politica DLP atunci când este evaluată. De exemplu, pentru un **Card de Credit politica** configurat cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa:</span><span class="sxs-lookup"><span data-stu-id="a5a0e-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="a5a0e-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddd) şi trebuie să treacă testul Luhn.</span><span class="sxs-lookup"><span data-stu-id="a5a0e-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="a5a0e-106">**[Model:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Model foarte complexă şi robustă care detectează cardurile de la toate marile branduri din întreaga lume, inclusiv Visa, Mastercard, descoperi Card, JCB, American Express, carduri cadou, şi carduri de cina.</span><span class="sxs-lookup"><span data-stu-id="a5a0e-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="a5a0e-107">**[Control:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, control Luhn</span><span class="sxs-lookup"><span data-stu-id="a5a0e-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="a5a0e-108">**[Definiţie:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** O politică de DLP este 85 % încrezător că a detectat acest tip de informaţii sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="a5a0e-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a5a0e-109">Funcţia Func_credit_card găseşte conţinut care se potriveşte model.</span><span class="sxs-lookup"><span data-stu-id="a5a0e-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="a5a0e-110">Este adevărată una dintre următoarele:</span><span class="sxs-lookup"><span data-stu-id="a5a0e-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="a5a0e-111">Se găseşte un cuvânt cheie la Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="a5a0e-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="a5a0e-112">Se găseşte un cuvânt cheie la Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="a5a0e-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="a5a0e-113">Funcţia Func_expiration_date constată o dată în formatul corect.</span><span class="sxs-lookup"><span data-stu-id="a5a0e-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="a5a0e-114">Control trece</span><span class="sxs-lookup"><span data-stu-id="a5a0e-114">The checksum passes</span></span>
    
    <span data-ttu-id="a5a0e-115">De exemplu, următoarea probă ar declanşa pentru o politică de număr de Card de Credit DLP:</span><span class="sxs-lookup"><span data-stu-id="a5a0e-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="a5a0e-116">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="a5a0e-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="a5a0e-117">Expira: 2/2009</span><span class="sxs-lookup"><span data-stu-id="a5a0e-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="a5a0e-118">Pentru mai multe informaţii despre ceea ce este necesar pentru un **Număr de Card de Credit** să fie detectată pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri arata pentru cardul de Credit #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a5a0e-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="a5a0e-119">Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a5a0e-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

