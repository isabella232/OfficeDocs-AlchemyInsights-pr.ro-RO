---
title: DlP regulă pentru SUA / Marea Britanie Pașaport Numărul nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507310"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="ba22b-102">Probleme cu DLP - SUA / Marea Britanie numerede pașaport</span><span class="sxs-lookup"><span data-stu-id="ba22b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="ba22b-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="ba22b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ba22b-104">**DLP probleme cu SUA / Marea Britanie numerede pașaport**</span><span class="sxs-lookup"><span data-stu-id="ba22b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="ba22b-105">Aveți probleme cu **prevenirea pierderilor de date (DLP)** care nu funcționează pentru conținut care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="ba22b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ba22b-106">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="ba22b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="ba22b-107">De exemplu, pentru o politică **de număr de pașaport SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze</span><span class="sxs-lookup"><span data-stu-id="ba22b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="ba22b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nouă cifre</span><span class="sxs-lookup"><span data-stu-id="ba22b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="ba22b-109">**[Model de model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nouă cifre consecutive</span><span class="sxs-lookup"><span data-stu-id="ba22b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="ba22b-110">**[Suma de control:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="ba22b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="ba22b-111">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="ba22b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ba22b-112">Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="ba22b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ba22b-113">Se găsește un cuvânt cheie din Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="ba22b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="ba22b-114">De exemplu, următorul eșantion ar declanșa politica **privind numărul pașaportului SUA/Regatul Unit:** numărul pașaportului SUA 123456789</span><span class="sxs-lookup"><span data-stu-id="ba22b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="ba22b-115">Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Marea Britanie să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce caută tipurile de informații sensibile pentru numărul pașaportului SUA/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ba22b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ba22b-116">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ba22b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  