---
title: DLP poate avea nevoie de un tip particularizat
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704501"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="51e33-102">DLP poate avea nevoie de un tip particularizat</span><span class="sxs-lookup"><span data-stu-id="51e33-102">DLP might need a custom type</span></span>

<span data-ttu-id="51e33-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="51e33-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="51e33-104">**DLP poate necesita un tip de informații particularizat**</span><span class="sxs-lookup"><span data-stu-id="51e33-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="51e33-105">Cu o politică de prevenire a pierderilor de date (DLP), puteți identifica și proteja datele sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="51e33-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="51e33-106">În unele scenarii, poate fi necesar să creați propriul tip de informații sensibile **particularizate** pentru a proteja datele organizației.</span><span class="sxs-lookup"><span data-stu-id="51e33-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="51e33-107">De exemplu, este posibil ca organizația să trebuiască să identifice și să protejeze ID-urile angajaților sau alte date într-un format specific orgului dvs. Dacă da, consultați următoarele articole pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="51e33-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="51e33-108">**Particularizarea unui tip de informații sensibile încorporate**</span><span class="sxs-lookup"><span data-stu-id="51e33-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="51e33-109">Dacă un tip de informații sensibile încorporat ar satisface nevoile dvs., cu doar câteva trucuri, puteți [personaliza un tip de informații sensibile încorporat](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="51e33-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="51e33-110">De exemplu, aveți posibilitatea să adăugați sau să eliminați cuvinte cheie sau să adăugați sau să eliminați dovezi justificative, ar fi o dată sau o adresă.</span><span class="sxs-lookup"><span data-stu-id="51e33-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="51e33-111">**Crearea unui tip de informații sensibile particularizate**</span><span class="sxs-lookup"><span data-stu-id="51e33-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="51e33-112">Dar dacă trebuie să identificați și să protejați cu totul un alt tip de informații sensibile, puteți [crea un tip de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) în interfața cu utilizatorul a Centrului de securitate & conformitate.</span><span class="sxs-lookup"><span data-stu-id="51e33-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="51e33-113">**Crearea unui tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell**</span><span class="sxs-lookup"><span data-stu-id="51e33-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="51e33-114">În cele din urmă, dacă interfața cu utilizatorul nu furnizează toate opțiunile de care aveți nevoie, aveți posibilitatea să [creați un tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="51e33-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="51e33-115">Începând cu un fișier XML, aveți posibilitatea să utilizați toate opțiunile disponibile.</span><span class="sxs-lookup"><span data-stu-id="51e33-115">By starting with an XML file, you can use every option available.</span></span>
