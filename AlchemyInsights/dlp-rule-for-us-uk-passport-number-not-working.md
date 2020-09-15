---
title: Regulă DLP pentru numărul de pașaport pentru SUA/Regatul Unit nu funcționează
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679236"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="2c7c7-102">Probleme cu numerele de pașaport DLP-US/UK</span><span class="sxs-lookup"><span data-stu-id="2c7c7-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="2c7c7-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="2c7c7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2c7c7-104">**Probleme DLP cu numerele de pașaport din SUA/Marea Britanie**</span><span class="sxs-lookup"><span data-stu-id="2c7c7-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="2c7c7-105">Întâmpinați probleme cu **prevenirea pierderii datelor (DLP)** care nu funcționează pentru conținutul care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații DLP sensibile în O365?</span><span class="sxs-lookup"><span data-stu-id="2c7c7-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2c7c7-106">Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="2c7c7-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2c7c7-107">De exemplu, pentru o politică de **număr pașaport din SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să fie declanșată</span><span class="sxs-lookup"><span data-stu-id="2c7c7-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="2c7c7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nouă cifre</span><span class="sxs-lookup"><span data-stu-id="2c7c7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="2c7c7-109">**[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nouă cifre consecutive</span><span class="sxs-lookup"><span data-stu-id="2c7c7-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="2c7c7-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nicio sumă de control</span><span class="sxs-lookup"><span data-stu-id="2c7c7-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2c7c7-111">**[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** O politică DLP este 75% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="2c7c7-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2c7c7-112">Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="2c7c7-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="2c7c7-113">S-a găsit un cuvânt cheie din Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="2c7c7-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="2c7c7-114">De exemplu, următorul eșantion ar declanșa politica pentru **numărul de pașapoarte din SUA/Marea Britanie** : pașaportul s.u.a. numărul 123456789</span><span class="sxs-lookup"><span data-stu-id="2c7c7-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="2c7c7-115">Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Regatul Unit să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile ne arată numărul de pașaport pentru SUA/Regatul Unit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="2c7c7-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="2c7c7-116">Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="2c7c7-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  