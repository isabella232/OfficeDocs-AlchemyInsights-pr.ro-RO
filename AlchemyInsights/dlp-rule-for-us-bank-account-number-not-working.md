---
title: Regulă DLP pentru numărul de cont bancar din SUA care nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932562"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="06c55-102">Dlp probleme cu sua numere de cont bancar</span><span class="sxs-lookup"><span data-stu-id="06c55-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="06c55-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="06c55-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="06c55-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="06c55-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="06c55-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="06c55-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="06c55-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="06c55-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="06c55-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="06c55-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="06c55-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="06c55-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="06c55-109">**Dlp probleme cu sua numere de cont bancar**</span><span class="sxs-lookup"><span data-stu-id="06c55-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="06c55-110">Aveți probleme cu **Data Loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de cont bancar din **SUA** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="06c55-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="06c55-111">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="06c55-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="06c55-112">De exemplu, pentru o politică **de număr de cont bancar din SUA** configuratcu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru regula pentru a declanșa:</span><span class="sxs-lookup"><span data-stu-id="06c55-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="06c55-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="06c55-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="06c55-114">**[Model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cifre consecutive.</span><span class="sxs-lookup"><span data-stu-id="06c55-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="06c55-115">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="06c55-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="06c55-116">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="06c55-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="06c55-117">Expresia regulată Regex_usa_bank_account_number găsește conținut care se potrivește cu modelul</span><span class="sxs-lookup"><span data-stu-id="06c55-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="06c55-118">Se găsește un cuvânt cheie din Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="06c55-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="06c55-119">De exemplu, următorul eșantion ar declanșa pentru politica **de număr de cont bancar din SUA:** Verificarea contului 78344011</span><span class="sxs-lookup"><span data-stu-id="06c55-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="06c55-120">Pentru mai multe informații despre ceea ce este necesar pentru un **număr de cont bancar din SUA** pentru a fi detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: Ce caută tipurile de informații [sensibile numărul de cont bancar din SUA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="06c55-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="06c55-121">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="06c55-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  