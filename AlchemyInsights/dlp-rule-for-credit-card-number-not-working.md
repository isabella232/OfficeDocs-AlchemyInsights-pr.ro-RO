---
title: Dlp Regulă pentru numărul cardului de credit nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932455"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="3fb4e-102">DLP probleme cu numerele de card de credit</span><span class="sxs-lookup"><span data-stu-id="3fb4e-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="3fb4e-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3fb4e-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3fb4e-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3fb4e-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3fb4e-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3fb4e-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3fb4e-109">**DLP probleme cu numerele de card de credit**</span><span class="sxs-lookup"><span data-stu-id="3fb4e-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="3fb4e-110">Aveți probleme cu **prevenirea pierderilor de date (DLP)** nu funcționează pentru conținut care conține un **număr de card de credit** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="3fb4e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3fb4e-111">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="3fb4e-112">De exemplu, pentru o **politică de card de credit** configurat cu un nivel de încredere de 85%, următoarele sunt evaluate și trebuie să fie detectate pentru regula pentru a declanșa:</span><span class="sxs-lookup"><span data-stu-id="3fb4e-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3fb4e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddddddddd) și trebuie să treacă testul Luhn.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="3fb4e-114">**[Model de model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Model foarte complex și robust, care detectează carduri de la toate mărcile importante din întreaga lume, inclusiv Visa, MasterCard, Discover Card, JCB, American Express, carduri cadou și carduri de restaurant.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="3fb4e-115">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, suma de control Luhn</span><span class="sxs-lookup"><span data-stu-id="3fb4e-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="3fb4e-116">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="3fb4e-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3fb4e-117">Funcția Func_credit_card găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3fb4e-118">Una dintre următoarele este adevărat:</span><span class="sxs-lookup"><span data-stu-id="3fb4e-118">One of the following is true:</span></span>

  - <span data-ttu-id="3fb4e-119">Se găsește un cuvânt cheie din Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="3fb4e-120">Se găsește un cuvânt cheie din Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="3fb4e-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="3fb4e-121">Funcția Func_expiration_date găsește o dată în formatul de dată corect.</span><span class="sxs-lookup"><span data-stu-id="3fb4e-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="3fb4e-122">Suma de control trece</span><span class="sxs-lookup"><span data-stu-id="3fb4e-122">The checksum passes</span></span>

    <span data-ttu-id="3fb4e-123">De exemplu, următorul eșantion ar declanșa pentru o politică de număr dlp card de credit:</span><span class="sxs-lookup"><span data-stu-id="3fb4e-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="3fb4e-124">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="3fb4e-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="3fb4e-125">Expiră: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3fb4e-125">Expires: 2/2009</span></span>

<span data-ttu-id="3fb4e-126">Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de card de credit** să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: Ce caută tipurile de informații [sensibile pentru cardul de credit#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="3fb4e-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3fb4e-127">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3fb4e-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  