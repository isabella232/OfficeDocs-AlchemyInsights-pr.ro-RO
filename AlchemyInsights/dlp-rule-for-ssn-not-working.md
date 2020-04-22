---
title: DlP regulă pentru SSN nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704097"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f8252-102">DLP probleme cu numerele de securitate socială</span><span class="sxs-lookup"><span data-stu-id="f8252-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f8252-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="f8252-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f8252-104">**DlP probleme cu SSNs**</span><span class="sxs-lookup"><span data-stu-id="f8252-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="f8252-105">Aveți probleme cu **data loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de securitate **socială (SSN)** atunci când utilizați un tip de informații sensibile în Office 365?</span><span class="sxs-lookup"><span data-stu-id="f8252-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="f8252-106">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP.</span><span class="sxs-lookup"><span data-stu-id="f8252-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f8252-107">De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze:</span><span class="sxs-lookup"><span data-stu-id="f8252-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f8252-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat</span><span class="sxs-lookup"><span data-stu-id="f8252-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f8252-109">**[Model de model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSN-uri în patru modele diferite:</span><span class="sxs-lookup"><span data-stu-id="f8252-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f8252-110">Func_ssn găsește SSN-uri cu formatare puternică pre-2011 care sunt formatate cu linițe sau spații (ddd-dddd SAU ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="f8252-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f8252-111">Func_unformatted_ssn găsește SSN-uri cu formatare puternică pre-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f8252-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f8252-112">Func_randomized_formatted_ssn găsește SSN-urile post-2011 care sunt formatate cu linițe sau spații (ddd-dd-dddd SAU ddd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="f8252-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f8252-113">Func_randomized_unformatted_ssn găsește SSN-urile post-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f8252-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f8252-114">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="f8252-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f8252-115">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="f8252-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f8252-116">[Funcția Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="f8252-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f8252-117">Se găsește un cuvânt cheie din [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="f8252-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="f8252-118">Exemple de cuvinte cheie includ: *Securitate socială, Securitate Socială#, Soc Sec ,SSN* .</span><span class="sxs-lookup"><span data-stu-id="f8252-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f8252-119">De exemplu, următorul eșantion ar declanșa pentru politica DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f8252-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f8252-120">Pentru mai multe informații despre ceea ce este necesar pentru ssn-uri pentru a fi detectate pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce tipuri de informații sensibile caută SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f8252-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f8252-121">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f8252-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  