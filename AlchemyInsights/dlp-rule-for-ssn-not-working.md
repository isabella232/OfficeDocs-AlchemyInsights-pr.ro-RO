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
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="6c140-102">DLP probleme cu numărul de securitate socială</span><span class="sxs-lookup"><span data-stu-id="6c140-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="6c140-103">Aveti probleme cu **Prevenirea pierderii datelor (DLP)** neactiv pentru conţinut care conţin un **Social Security Number (SSN)** atunci când se utilizează un tip de informaţii sensibile din Office 365?</span><span class="sxs-lookup"><span data-stu-id="6c140-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="6c140-104">Dacă este aşa, asiguraţi-vă că conţinut conţine informaţiile necesare pentru ceea ce este în căutarea DLP politica.</span><span class="sxs-lookup"><span data-stu-id="6c140-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="6c140-105">De exemplu, pentru o politică de SSN configurat cu un nivel de încredere de 85 %, următoarele sunt evaluate şi trebuie să fie detectat de regulă pentru a declanşa:</span><span class="sxs-lookup"><span data-stu-id="6c140-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6c140-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, care poate fi într-un model formatate sau neformatate</span><span class="sxs-lookup"><span data-stu-id="6c140-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="6c140-107">**[Model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru functii uite pentru SSNs în patru modele diferite:</span><span class="sxs-lookup"><span data-stu-id="6c140-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="6c140-108">Func_ssn gaseste SSNs cu pre-2011 puternic formatări care sunt formatate cu liniuţe sau spatii (val de ddd dd OR ddd dd vi)</span><span class="sxs-lookup"><span data-stu-id="6c140-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6c140-109">Func_unformatted_ssn gaseste SSNs cu pre-2011 puternic formatări care sunt neformatat ca nouă cifre consecutive (Elena)</span><span class="sxs-lookup"><span data-stu-id="6c140-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="6c140-110">Func_randomized_formatted_ssn constată post-2011 SSNs care sunt formatate cu liniuţe sau spatii (val de ddd dd OR ddd dd vi)</span><span class="sxs-lookup"><span data-stu-id="6c140-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6c140-111">Func_randomized_unformatted_ssn constată post-2011 SSNs care sunt neformatat ca nouă cifre consecutive (Elena)</span><span class="sxs-lookup"><span data-stu-id="6c140-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="6c140-112">**[Control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nu, nu există nici o sumă de control</span><span class="sxs-lookup"><span data-stu-id="6c140-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="6c140-113">**[Definiţie:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** O politică de DLP este 85 % încrezător că a detectat acest tip de informaţii sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="6c140-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6c140-114">[Funcţia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) găseşte conţinut care se potriveşte model.</span><span class="sxs-lookup"><span data-stu-id="6c140-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6c140-115">Se găseşte un cuvânt cheie la [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="6c140-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="6c140-116">Exemple de cuvinte cheie include: *securitate socială, securitate socială #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="6c140-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="6c140-117">De exemplu, următoarea probă ar declanşa pentru politica DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="6c140-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="6c140-118">Pentru mai multe informaţii despre ceea ce este necesar pentru SSNs să fie detectate pentru conţinutul dvs., a se vedea secţiunea următoare în acest articol: [Ce Sensitive informaţii tipuri uite pentru SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="6c140-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="6c140-119">Folosind un tip de diferite informaţii sensibile predefinite, consultaţi următorul articol pentru informaţii pe ceea ce este necesar pentru alte tipuri: [ce Sensitive informaţii tipuri caute](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6c140-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  