---
title: Regulă DLP pentru numărul cardului de credit nu funcționează
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679453"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="c92a3-102">Probleme DLP cu numerele cardului de credit</span><span class="sxs-lookup"><span data-stu-id="c92a3-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="c92a3-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="c92a3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c92a3-104">**Probleme DLP cu numerele cardului de credit**</span><span class="sxs-lookup"><span data-stu-id="c92a3-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="c92a3-105">Aveți probleme cu **prevenirea pierderii datelor (DLP)** nu funcționează pentru conținutul care conține un **număr de card de credit** atunci când utilizați un tip de informații DLP sensibile în O365?</span><span class="sxs-lookup"><span data-stu-id="c92a3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c92a3-106">Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="c92a3-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="c92a3-107">De exemplu, pentru o **politică a cardului de credit** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:</span><span class="sxs-lookup"><span data-stu-id="c92a3-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c92a3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddd) și trebuie să treacă testul Luhn.</span><span class="sxs-lookup"><span data-stu-id="c92a3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="c92a3-109">**[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Model foarte complex și robust care detectează cărți din toate marile branduri din întreaga lume, inclusiv Visa, MasterCard, Discover card, JCB, American Express, Gift Cards și Diner Cards.</span><span class="sxs-lookup"><span data-stu-id="c92a3-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="c92a3-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, checksum Luhn</span><span class="sxs-lookup"><span data-stu-id="c92a3-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="c92a3-111">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** O politică DLP este 85% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="c92a3-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c92a3-112">Funcția Func_credit_card găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="c92a3-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c92a3-113">Una dintre următoarele este True:</span><span class="sxs-lookup"><span data-stu-id="c92a3-113">One of the following is true:</span></span>

  - <span data-ttu-id="c92a3-114">S-a găsit un cuvânt cheie din Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="c92a3-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="c92a3-115">S-a găsit un cuvânt cheie din Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="c92a3-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="c92a3-116">Funcția Func_expiration_date găsește o dată în formatul de dată potrivit.</span><span class="sxs-lookup"><span data-stu-id="c92a3-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="c92a3-117">Valoarea de control trece</span><span class="sxs-lookup"><span data-stu-id="c92a3-117">The checksum passes</span></span>

    <span data-ttu-id="c92a3-118">De exemplu, următorul eșantion ar declanșa o politică de număr a cardului de credit DLP:</span><span class="sxs-lookup"><span data-stu-id="c92a3-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="c92a3-119">Viză: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="c92a3-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="c92a3-120">Expiră: 2/2009</span><span class="sxs-lookup"><span data-stu-id="c92a3-120">Expires: 2/2009</span></span>

<span data-ttu-id="c92a3-121">Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de card de credit** să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile caută cardul de credit #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="c92a3-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="c92a3-122">Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c92a3-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  