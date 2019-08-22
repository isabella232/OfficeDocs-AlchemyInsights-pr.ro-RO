---
title: DLP nu funcţionează conform aşteptărilor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530303"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="142f9-102">DLP nu funcţionează conform aşteptărilor</span><span class="sxs-lookup"><span data-stu-id="142f9-102">DLP not working as expected</span></span>

<span data-ttu-id="142f9-103">Au probleme cu **Prevenirea pierderii datelor (DLP)** în Office 365 nu funcţionează conform aşteptărilor?</span><span class="sxs-lookup"><span data-stu-id="142f9-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="142f9-104">Dacă este aşa, asiguraţi-vă că vă **DLP politica** este configurat corect, şi că datele dumneavoastră conţine ceea ce **Politica de DLP** este în căutarea pentru atunci când ea este evaluate.</span><span class="sxs-lookup"><span data-stu-id="142f9-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="142f9-105">**Configurarea DLP**</span><span class="sxs-lookup"><span data-stu-id="142f9-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="142f9-106">DLP politici vă identifica şi de a proteja informaţiile sensibile din organizaţie.</span><span class="sxs-lookup"><span data-stu-id="142f9-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="142f9-107">La configurare DLP politici, utilizaţi informaţiile [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="142f9-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="142f9-108">**Ce arata DLP politici**</span><span class="sxs-lookup"><span data-stu-id="142f9-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="142f9-109">Atunci când se utilizează **built-in informaţiile sensibile tipuri** în Office 365 securitatea şi conformitatea center, DLP politici caute modele specifice şi elemente atunci când detectează aceste tipuri sensibile.</span><span class="sxs-lookup"><span data-stu-id="142f9-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="142f9-110">**Clădire-înăuntru informaţii sensibile tipuri**</span><span class="sxs-lookup"><span data-stu-id="142f9-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="142f9-111">Pentru informații privind tipurile de built-in sensibile şi ceea ce arata o politică DLP atunci când detectează tipul sensibil, a se vedea: [ce tipuri de informaţii sensibile caută](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="142f9-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="142f9-112">**Tipurile de informaţii sensibile personalizate**</span><span class="sxs-lookup"><span data-stu-id="142f9-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="142f9-113">Dacă încercaţi să creaţi tipuri personalizate de informaţii sensibile, utilizaţi următorul articol pentru informaţii despre cum să creaţi un tip sensibil personalizate: [creaţi un tip personalizat de informaţii sensibile](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="142f9-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="142f9-114">**O politică de DLP de testare**</span><span class="sxs-lookup"><span data-stu-id="142f9-114">**Test a DLP policy**</span></span>

<span data-ttu-id="142f9-115">Pentru a testa datele cu un tip de informaţii sensibile predefinite sau particularizate, utilizaţi opţiunea **tip de testare** în conformitate cu **clasificările** > **tipuri de informaţii sensibile**.</span><span class="sxs-lookup"><span data-stu-id="142f9-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="142f9-116">Pentru mai multe informații, vedeți [tipuri de informaţii sensibile personalizate Test](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="142f9-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="142f9-117">**Rapoarte**</span><span class="sxs-lookup"><span data-stu-id="142f9-117">**Reports**</span></span>
  
- <span data-ttu-id="142f9-118">Obţine date sensibile intuiţii cu [DLP rapoarte.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="142f9-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="142f9-119">Vedea detaliile specifice ale evenimentul cu un [Raport de Incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="142f9-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
