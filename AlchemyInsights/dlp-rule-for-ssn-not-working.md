---
title: Regulă DLP pentru SSN nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679381"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="03ad8-102">Probleme DLP cu numerele de securitate socială</span><span class="sxs-lookup"><span data-stu-id="03ad8-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="03ad8-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="03ad8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="03ad8-104">**Probleme DLP cu SSNs**</span><span class="sxs-lookup"><span data-stu-id="03ad8-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="03ad8-105">Întâmpinați probleme cu **prevenirea pierderii datelor (DLP)** care nu funcționează pentru conținutul care conține un **număr de securitate socială (SSN)** atunci când utilizați un tip de informații sensibile în Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="03ad8-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="03ad8-106">Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP.</span><span class="sxs-lookup"><span data-stu-id="03ad8-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="03ad8-107">De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:</span><span class="sxs-lookup"><span data-stu-id="03ad8-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="03ad8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat</span><span class="sxs-lookup"><span data-stu-id="03ad8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="03ad8-109">**[Model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSNs în patru modele diferite:</span><span class="sxs-lookup"><span data-stu-id="03ad8-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="03ad8-110">Func_ssn găsește SSNs cu o formatare puternică pre-2011, care este formatată cu linii întrerupte sau spații (ddd-dd-dddd sau ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="03ad8-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="03ad8-111">Func_unformatted_ssn găsește SSNs cu o formatare puternică pre-2011, care este neformatată ca nouă cifre consecutive (gales)</span><span class="sxs-lookup"><span data-stu-id="03ad8-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="03ad8-112">Func_randomized_formatted_ssn găsește SSNs post-2011 care sunt formatate cu linii întrerupte sau spații (ddd-dd-dddd sau ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="03ad8-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="03ad8-113">Func_randomized_unformatted_ssn găsește SSNs post-2011 care sunt neformatate ca nouă cifre consecutive (gales)</span><span class="sxs-lookup"><span data-stu-id="03ad8-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="03ad8-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nu, nu există nicio sumă de control</span><span class="sxs-lookup"><span data-stu-id="03ad8-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="03ad8-115">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** O politică DLP este 85% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="03ad8-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="03ad8-116">[Funcția Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="03ad8-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="03ad8-117">S-a găsit un cuvânt cheie din [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="03ad8-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="03ad8-118">Exemple de cuvinte cheie includ:  *securitate socială, securitate socială #, soc sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="03ad8-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="03ad8-119">De exemplu, următorul eșantion ar declanșa politica DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="03ad8-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="03ad8-120">Pentru mai multe informații despre ceea ce este necesar pentru ca SSNs să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce caută tipurile de informații sensibile pentru SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="03ad8-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="03ad8-121">Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="03ad8-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  