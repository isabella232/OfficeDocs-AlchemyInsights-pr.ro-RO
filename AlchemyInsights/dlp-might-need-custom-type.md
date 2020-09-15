---
title: Este posibil ca DLP să aibă nevoie de un tip particularizat
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712196"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="83d80-102">Este posibil ca DLP să aibă nevoie de un tip particularizat</span><span class="sxs-lookup"><span data-stu-id="83d80-102">DLP might need a custom type</span></span>

<span data-ttu-id="83d80-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="83d80-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="83d80-104">**DLP poate necesita un tip de informații particularizat**</span><span class="sxs-lookup"><span data-stu-id="83d80-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="83d80-105">Cu o politică de prevenire a pierderii datelor (DLP), puteți să identificați și să protejați datele sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="83d80-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="83d80-106">În unele scenarii, poate fi necesar să creați propriul tip de informații sensibile **particularizat** pentru a proteja datele organizației.</span><span class="sxs-lookup"><span data-stu-id="83d80-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="83d80-107">De exemplu, poate fi necesar ca organizația să identifice și să protejeze ID-urile angajaților sau alte date în unele formate specifice organizației dvs. Dacă da, consultați următoarele articole pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="83d80-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="83d80-108">**Particularizarea unui tip de informații sensibile predefinite**</span><span class="sxs-lookup"><span data-stu-id="83d80-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="83d80-109">Dacă un tip de informație sensibil încorporat v-ar satisface nevoile cu doar câteva ajustări, puteți să [particularizați un tip de informații sensibile predefinite](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="83d80-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="83d80-110">De exemplu, puteți să adăugați sau să eliminați cuvinte cheie sau să adăugați sau să eliminați dovezi justificative, cum ar fi o dată sau o adresă.</span><span class="sxs-lookup"><span data-stu-id="83d80-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="83d80-111">**Crearea unui tip de informații sensibile la comandă**</span><span class="sxs-lookup"><span data-stu-id="83d80-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="83d80-112">Dar, dacă trebuie să identificați și să protejați cu totul un alt tip de informații sensibile, puteți să [Creați un tip de informații sensibile particularizat](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) în interfața de utilizator a centrului de conformitate & de securitate.</span><span class="sxs-lookup"><span data-stu-id="83d80-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="83d80-113">**Crearea unui tip de informații sensibile cu caracter particularizat în securitatea & în centrul de conformitate PowerShell**</span><span class="sxs-lookup"><span data-stu-id="83d80-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="83d80-114">În cele din urmă, dacă interfața de utilizator nu furnizează toate opțiunile de care aveți nevoie, puteți să [Creați un tip de informații sensibile particularizat în securitate & PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="83d80-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="83d80-115">Începând cu un fișier XML, puteți utiliza toate opțiunile disponibile.</span><span class="sxs-lookup"><span data-stu-id="83d80-115">By starting with an XML file, you can use every option available.</span></span>
