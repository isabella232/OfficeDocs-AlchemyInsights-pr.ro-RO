---
title: DLP nu funcționează conform așteptărilor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507490"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5ae96-102">DLP nu funcționează conform așteptărilor</span><span class="sxs-lookup"><span data-stu-id="5ae96-102">DLP not working as expected</span></span>

<span data-ttu-id="5ae96-103">**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="5ae96-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="5ae96-104">**Configurarea DLP**</span><span class="sxs-lookup"><span data-stu-id="5ae96-104">**Setting up DLP**</span></span>

<span data-ttu-id="5ae96-105">Aveți probleme cu **prevenirea pierderilor de date (DLP)** în Office 365 nu funcționează conform așteptărilor?</span><span class="sxs-lookup"><span data-stu-id="5ae96-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5ae96-106">Dacă da, asigurați-vă că **politica DLP** este configurat corect și că datele conține ceea ce **politica DLP** este în căutarea atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="5ae96-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5ae96-107">Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="5ae96-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5ae96-108">Pentru a parametriza politicile DLP, utilizați informațiile [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="5ae96-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5ae96-109">**Ce caută politicile DLP**</span><span class="sxs-lookup"><span data-stu-id="5ae96-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5ae96-110">Atunci când utilizați **tipurile de informații sensibile încorporate** în centrele de securitate și conformitate, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.</span><span class="sxs-lookup"><span data-stu-id="5ae96-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5ae96-111">**Tipuri de informații sensibile încorporate**</span><span class="sxs-lookup"><span data-stu-id="5ae96-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5ae96-112">Pentru informații despre tipurile sensibile încorporate și ce caută o politică DLP la detectarea tipului Sensibil, consultați: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="5ae96-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="5ae96-113">**Tipuri de informații sensibile particularizate**</span><span class="sxs-lookup"><span data-stu-id="5ae96-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5ae96-114">Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre se creează un tip sensibil particularizat: [Creați un tip de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5ae96-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5ae96-115">**Testarea unei politici DLP**</span><span class="sxs-lookup"><span data-stu-id="5ae96-115">**Test a DLP policy**</span></span>

<span data-ttu-id="5ae96-116">Pentru a testa datele cu un tip de informații sensibile predefinite sau particularizate, utilizați opțiunea **Tip test** din **Clasificări**  >  **Tipuri de informații sensibile**.</span><span class="sxs-lookup"><span data-stu-id="5ae96-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5ae96-117">Pentru mai multe informații, consultați [Testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="5ae96-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5ae96-118">**Rapoarte**</span><span class="sxs-lookup"><span data-stu-id="5ae96-118">**Reports**</span></span>
  
- <span data-ttu-id="5ae96-119">Obțineți informații sensibile despre date cu [rapoarteLE DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5ae96-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5ae96-120">A se vedea detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="5ae96-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
