---
title: Dlp Regulă pentru numărul cardului de credit nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704213"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="64453-102">DLP probleme cu numerele de card de credit</span><span class="sxs-lookup"><span data-stu-id="64453-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="64453-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="64453-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="64453-104">**DLP probleme cu numerele de card de credit**</span><span class="sxs-lookup"><span data-stu-id="64453-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="64453-105">Aveți probleme cu **prevenirea pierderilor de date (DLP)** nu funcționează pentru conținut care conține un **număr de card de credit** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="64453-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="64453-106">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="64453-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="64453-107">De exemplu, pentru o **politică de card de credit** configurat cu un nivel de încredere de 85%, următoarele sunt evaluate și trebuie să fie detectate pentru regula pentru a declanșa:</span><span class="sxs-lookup"><span data-stu-id="64453-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="64453-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddddddddd) și trebuie să treacă testul Luhn.</span><span class="sxs-lookup"><span data-stu-id="64453-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="64453-109">**[Model de model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Model foarte complex și robust, care detectează carduri de la toate mărcile importante din întreaga lume, inclusiv Visa, MasterCard, Discover Card, JCB, American Express, carduri cadou și carduri de restaurant.</span><span class="sxs-lookup"><span data-stu-id="64453-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="64453-110">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, suma de control Luhn</span><span class="sxs-lookup"><span data-stu-id="64453-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="64453-111">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="64453-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="64453-112">Funcția Func_credit_card găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="64453-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="64453-113">Una dintre următoarele este adevărat:</span><span class="sxs-lookup"><span data-stu-id="64453-113">One of the following is true:</span></span>

  - <span data-ttu-id="64453-114">Se găsește un cuvânt cheie din Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="64453-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="64453-115">Se găsește un cuvânt cheie din Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="64453-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="64453-116">Funcția Func_expiration_date găsește o dată în formatul de dată corect.</span><span class="sxs-lookup"><span data-stu-id="64453-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="64453-117">Suma de control trece</span><span class="sxs-lookup"><span data-stu-id="64453-117">The checksum passes</span></span>

    <span data-ttu-id="64453-118">De exemplu, următorul eșantion ar declanșa pentru o politică de număr dlp card de credit:</span><span class="sxs-lookup"><span data-stu-id="64453-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="64453-119">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="64453-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="64453-120">Expiră: 2/2009</span><span class="sxs-lookup"><span data-stu-id="64453-120">Expires: 2/2009</span></span>

<span data-ttu-id="64453-121">Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de card de credit** să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: Ce caută tipurile de informații [sensibile pentru cardul de credit#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="64453-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="64453-122">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="64453-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  