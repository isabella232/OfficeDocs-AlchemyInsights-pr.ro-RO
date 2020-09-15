---
title: DLP nu funcționează așa cum vă așteptați
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679705"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="73839-102">DLP nu funcționează așa cum vă așteptați</span><span class="sxs-lookup"><span data-stu-id="73839-102">DLP not working as expected</span></span>

<span data-ttu-id="73839-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="73839-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="73839-104">**Configurarea DLP**</span><span class="sxs-lookup"><span data-stu-id="73839-104">**Setting up DLP**</span></span>

<span data-ttu-id="73839-105">Aveți probleme cu **prevenirea pierderii datelor (DLP)** în Office 365 nu funcționează așa cum vă așteptați?</span><span class="sxs-lookup"><span data-stu-id="73839-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="73839-106">Dacă este așa, asigurați-vă că **Politica DLP** este configurată corect și că datele conțin ceea ce caută **Politica DLP** atunci când este evaluată.</span><span class="sxs-lookup"><span data-stu-id="73839-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="73839-107">Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="73839-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="73839-108">Pentru a configura politicile DLP, utilizați informațiile de [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="73839-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="73839-109">**Ce caută politicile DLP**</span><span class="sxs-lookup"><span data-stu-id="73839-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="73839-110">Atunci când utilizați **tipurile de informații sensibile predefinite** din centrele de securitate și conformitate, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.</span><span class="sxs-lookup"><span data-stu-id="73839-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="73839-111">**Tipuri de informații sensibile predefinite**</span><span class="sxs-lookup"><span data-stu-id="73839-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="73839-112">Pentru informații despre tipurile sensibile predefinite și ce caută o politică DLP atunci când detectează tipul sensibil, consultați: [ce caută tipurile sensibile de informații](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="73839-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="73839-113">**Tipuri de informații sensibile la comandă**</span><span class="sxs-lookup"><span data-stu-id="73839-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="73839-114">Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre cum să creați un tip sensibil particularizat: [Creați un tip de informații sensibile la comandă](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="73839-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="73839-115">**Testarea unei politici DLP**</span><span class="sxs-lookup"><span data-stu-id="73839-115">**Test a DLP policy**</span></span>

<span data-ttu-id="73839-116">Pentru a testa datele cu un tip de informație predefinit sau particularizat, utilizați opțiunea **tip test** **sub**  >  **Categorii informații sensibile**.</span><span class="sxs-lookup"><span data-stu-id="73839-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="73839-117">Pentru mai multe informații, consultați [testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="73839-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="73839-118">**Rapoarte**</span><span class="sxs-lookup"><span data-stu-id="73839-118">**Reports**</span></span>
  
- <span data-ttu-id="73839-119">Obțineți informații sensibile despre date cu [rapoartele DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="73839-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="73839-120">Vedeți detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="73839-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
