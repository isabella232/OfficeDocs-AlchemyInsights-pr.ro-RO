---
title: DlP regulă pentru SUA / Marea Britanie Pașaport Numărul nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931274"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="93d5f-102">Probleme cu DLP - SUA / Marea Britanie numerede pașaport</span><span class="sxs-lookup"><span data-stu-id="93d5f-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="93d5f-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="93d5f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="93d5f-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="93d5f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="93d5f-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="93d5f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="93d5f-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="93d5f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="93d5f-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="93d5f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="93d5f-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="93d5f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="93d5f-109">**DLP probleme cu SUA / Marea Britanie numerede pașaport**</span><span class="sxs-lookup"><span data-stu-id="93d5f-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="93d5f-110">Aveți probleme cu **prevenirea pierderilor de date (DLP)** care nu funcționează pentru conținut care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații sensibile DLP în O365?</span><span class="sxs-lookup"><span data-stu-id="93d5f-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="93d5f-111">Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="93d5f-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="93d5f-112">De exemplu, pentru o politică **de număr de pașaport SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze</span><span class="sxs-lookup"><span data-stu-id="93d5f-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="93d5f-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nouă cifre</span><span class="sxs-lookup"><span data-stu-id="93d5f-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="93d5f-114">**[Model de model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nouă cifre consecutive</span><span class="sxs-lookup"><span data-stu-id="93d5f-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="93d5f-115">**[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici un Checksum</span><span class="sxs-lookup"><span data-stu-id="93d5f-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="93d5f-116">**[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:</span><span class="sxs-lookup"><span data-stu-id="93d5f-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="93d5f-117">Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.</span><span class="sxs-lookup"><span data-stu-id="93d5f-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="93d5f-118">Se găsește un cuvânt cheie din Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="93d5f-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="93d5f-119">De exemplu, următorul eșantion ar declanșa politica **privind numărul pașaportului SUA/Regatul Unit:** numărul pașaportului SUA 123456789</span><span class="sxs-lookup"><span data-stu-id="93d5f-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="93d5f-120">Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Marea Britanie să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce caută tipurile de informații sensibile pentru numărul pașaportului SUA/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="93d5f-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="93d5f-121">Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="93d5f-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  