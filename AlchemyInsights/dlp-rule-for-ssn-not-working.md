---
title: DlP regulă pentru SSN nu funcționează
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932547"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="c5aa9-102">DLP probleme cu numerele de securitate socială</span><span class="sxs-lookup"><span data-stu-id="c5aa9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="c5aa9-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c5aa9-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c5aa9-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c5aa9-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c5aa9-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c5aa9-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c5aa9-109">**DlP probleme cu SSNs**</span><span class="sxs-lookup"><span data-stu-id="c5aa9-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="c5aa9-110">Aveți probleme cu **data loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de securitate **socială (SSN)** atunci când utilizați un tip de informații sensibile în Office 365?</span><span class="sxs-lookup"><span data-stu-id="c5aa9-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="c5aa9-111">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="c5aa9-112">De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze:</span><span class="sxs-lookup"><span data-stu-id="c5aa9-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c5aa9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat</span><span class="sxs-lookup"><span data-stu-id="c5aa9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="c5aa9-114">**[Model de model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSN-uri în patru modele diferite:</span><span class="sxs-lookup"><span data-stu-id="c5aa9-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="c5aa9-115">Func_ssn găsește SSN-uri cu formatare puternică pre-2011 care sunt formatate cu linițe sau spații (ddd-dddd SAU ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c5aa9-116">Func_unformatted_ssn găsește SSN-uri cu formatare puternică pre-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="c5aa9-117">Func_randomized_formatted_ssn găsește SSN-urile post-2011 care sunt formatate cu linițe sau spații (ddd-dd-dddd SAU ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c5aa9-118">Func_randomized_unformatted_ssn găsește SSN-urile post-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="c5aa9-119">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="c5aa9-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="c5aa9-120">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="c5aa9-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c5aa9-121">[Funcția Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="c5aa9-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c5aa9-122">Se găsește un cuvânt cheie din [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="c5aa9-123">Exemple de cuvinte cheie includ: *Securitate socială, Securitate Socială#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="c5aa9-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="c5aa9-124">De exemplu, următorul eșantion ar declanșa pentru politica DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="c5aa9-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="c5aa9-125">Pentru mai multe informații despre ceea ce este necesar pentru ssn-uri pentru a fi detectate pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce tipuri de informații sensibile caută SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="c5aa9-126">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c5aa9-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  