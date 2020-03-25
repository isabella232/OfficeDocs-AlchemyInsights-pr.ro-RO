---
title: DLP poate avea nevoie de un tip particularizat
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932670"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d6f24-102">DLP poate avea nevoie de un tip particularizat</span><span class="sxs-lookup"><span data-stu-id="d6f24-102">DLP might need a custom type</span></span>

<span data-ttu-id="d6f24-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="d6f24-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d6f24-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="d6f24-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d6f24-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="d6f24-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d6f24-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="d6f24-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d6f24-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="d6f24-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d6f24-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="d6f24-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d6f24-109">**DLP poate necesita un tip de informații particularizat**</span><span class="sxs-lookup"><span data-stu-id="d6f24-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d6f24-110">Cu o politică de prevenire a pierderilor de date (DLP), puteți identifica și proteja datele sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="d6f24-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d6f24-111">În unele scenarii, poate fi necesar să creați propriul tip de informații sensibile **particularizate** pentru a proteja datele organizației.</span><span class="sxs-lookup"><span data-stu-id="d6f24-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d6f24-112">De exemplu, este posibil ca organizația să trebuiască să identifice și să protejeze ID-urile angajaților sau alte date într-un format specific orgului dvs. Dacă da, consultați următoarele articole pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="d6f24-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d6f24-113">**Particularizarea unui tip de informații sensibile încorporate**</span><span class="sxs-lookup"><span data-stu-id="d6f24-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d6f24-114">Dacă un tip de informații sensibile încorporat ar satisface nevoile dvs., cu doar câteva trucuri, puteți [personaliza un tip de informații sensibile încorporat](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d6f24-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d6f24-115">De exemplu, aveți posibilitatea să adăugați sau să eliminați cuvinte cheie sau să adăugați sau să eliminați dovezi justificative, ar fi o dată sau o adresă.</span><span class="sxs-lookup"><span data-stu-id="d6f24-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d6f24-116">**Crearea unui tip de informații sensibile particularizate**</span><span class="sxs-lookup"><span data-stu-id="d6f24-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d6f24-117">Dar dacă trebuie să identificați și să protejați cu totul un alt tip de informații sensibile, puteți [crea un tip de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) în interfața cu utilizatorul a Centrului de securitate & conformitate.</span><span class="sxs-lookup"><span data-stu-id="d6f24-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d6f24-118">**Crearea unui tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell**</span><span class="sxs-lookup"><span data-stu-id="d6f24-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d6f24-119">În cele din urmă, dacă interfața cu utilizatorul nu furnizează toate opțiunile de care aveți nevoie, aveți posibilitatea să [creați un tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d6f24-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d6f24-120">Începând cu un fișier XML, aveți posibilitatea să utilizați toate opțiunile disponibile.</span><span class="sxs-lookup"><span data-stu-id="d6f24-120">By starting with an XML file, you can use every option available.</span></span>
