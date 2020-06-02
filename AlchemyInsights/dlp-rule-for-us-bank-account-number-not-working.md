---
title: Regulă DLP pentru numărul de cont bancar din SUA care nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507346"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="16d2f-102">Dlp probleme cu sua numere de cont bancar</span><span class="sxs-lookup"><span data-stu-id="16d2f-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="16d2f-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="16d2f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="16d2f-104">**Dlp probleme cu sua numere de cont bancar**</span><span class="sxs-lookup"><span data-stu-id="16d2f-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="16d2f-105">Aveți probleme cu **Data Loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de cont bancar din **SUA** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="16d2f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="16d2f-106">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="16d2f-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="16d2f-107">De exemplu, pentru o politică **de număr de cont bancar din SUA** configuratcu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru regula pentru a declanșa:</span><span class="sxs-lookup"><span data-stu-id="16d2f-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="16d2f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="16d2f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="16d2f-109">**[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 cifre consecutive.</span><span class="sxs-lookup"><span data-stu-id="16d2f-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="16d2f-110">**[Suma de control:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="16d2f-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="16d2f-111">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="16d2f-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="16d2f-112">Expresia regulată Regex_usa_bank_account_number găsește conținut care se potrivește cu modelul</span><span class="sxs-lookup"><span data-stu-id="16d2f-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="16d2f-113">Se găsește un cuvânt cheie din Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="16d2f-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="16d2f-114">De exemplu, următorul eșantion ar declanșa pentru politica **de număr de cont bancar din SUA:** Verificarea contului 78344011</span><span class="sxs-lookup"><span data-stu-id="16d2f-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="16d2f-115">Pentru mai multe informații despre ceea ce este necesar pentru un **număr de cont bancar din SUA** pentru a fi detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: Ce caută tipurile de informații [sensibile numărul de cont bancar din SUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="16d2f-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="16d2f-116">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="16d2f-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  