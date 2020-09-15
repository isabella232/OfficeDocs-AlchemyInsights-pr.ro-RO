---
title: Regulă DLP pentru numărul de cont bancar din S.U.A. nu funcționează
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679308"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="73842-102">Probleme DLP cu numerele conturilor bancare din SUA</span><span class="sxs-lookup"><span data-stu-id="73842-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="73842-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="73842-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="73842-104">**Probleme DLP cu numerele conturilor bancare din SUA**</span><span class="sxs-lookup"><span data-stu-id="73842-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="73842-105">Aveți probleme cu **prevenirea pierderii datelor (DLP)** nu funcționează pentru conținutul care conține un **număr de cont bancar din s.u.a.** atunci când utilizați un tip de informații DLP sensibile în O365?</span><span class="sxs-lookup"><span data-stu-id="73842-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="73842-106">Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="73842-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="73842-107">De exemplu, pentru o politică de **număr de cont bancar din s.u.a.** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:</span><span class="sxs-lookup"><span data-stu-id="73842-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="73842-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="73842-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="73842-109">**[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 cifre consecutive.</span><span class="sxs-lookup"><span data-stu-id="73842-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="73842-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nicio sumă de control</span><span class="sxs-lookup"><span data-stu-id="73842-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="73842-111">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** O politică DLP este 75% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="73842-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="73842-112">Expresia obișnuită Regex_usa_bank_account_number găsește conținut care se potrivește cu modelul</span><span class="sxs-lookup"><span data-stu-id="73842-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="73842-113">S-a găsit un cuvânt cheie din Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="73842-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="73842-114">De exemplu, următorul eșantion ar declanșa Politica de **număr al contului bancar din SUA** : verificarea contului 78344011</span><span class="sxs-lookup"><span data-stu-id="73842-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="73842-115">Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de cont bancar din s.u.a.** să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile ne caută numărul de cont bancar din SUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="73842-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="73842-116">Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="73842-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  