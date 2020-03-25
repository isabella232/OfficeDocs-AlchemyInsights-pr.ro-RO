---
title: DLP nu funcționează conform așteptărilor
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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932634"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="1badc-102">DLP nu funcționează conform așteptărilor</span><span class="sxs-lookup"><span data-stu-id="1badc-102">DLP not working as expected</span></span>

<span data-ttu-id="1badc-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="1badc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1badc-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="1badc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1badc-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="1badc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1badc-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="1badc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1badc-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="1badc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1badc-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="1badc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="1badc-109">**Configurarea DLP**</span><span class="sxs-lookup"><span data-stu-id="1badc-109">**Setting up DLP**</span></span>

<span data-ttu-id="1badc-110">Aveți probleme cu **prevenirea pierderilor de date (DLP)** în Office 365 nu funcționează conform așteptărilor?</span><span class="sxs-lookup"><span data-stu-id="1badc-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="1badc-111">Dacă da, asigurați-vă că **politica DLP** este configurat corect și că datele conține ceea ce **politica DLP** este în căutarea atunci când este evaluat.</span><span class="sxs-lookup"><span data-stu-id="1badc-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="1badc-112">Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="1badc-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="1badc-113">Pentru a parametriza politicile DLP, utilizați informațiile [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="1badc-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="1badc-114">**Ce caută politicile DLP**</span><span class="sxs-lookup"><span data-stu-id="1badc-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="1badc-115">Atunci când utilizați **tipurile de informații sensibile predefinite** în Centrul de securitate și conformitate Office 365, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.</span><span class="sxs-lookup"><span data-stu-id="1badc-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="1badc-116">**Tipuri de informații sensibile încorporate**</span><span class="sxs-lookup"><span data-stu-id="1badc-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="1badc-117">Pentru informații despre tipurile sensibile încorporate și ce caută o politică DLP la detectarea tipului Sensibil, consultați: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="1badc-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="1badc-118">**Tipuri de informații sensibile particularizate**</span><span class="sxs-lookup"><span data-stu-id="1badc-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="1badc-119">Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre se creează un tip sensibil particularizat: [Creați un tip de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1badc-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="1badc-120">**Testarea unei politici DLP**</span><span class="sxs-lookup"><span data-stu-id="1badc-120">**Test a DLP policy**</span></span>

<span data-ttu-id="1badc-121">Pentru a testa datele cu un tip de informații sensibile predefinite sau particularizate, utilizați opțiunea **Tip test** din **Clasificări** > **Tipuri de informații sensibile**.</span><span class="sxs-lookup"><span data-stu-id="1badc-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="1badc-122">Pentru mai multe informații, consultați [Testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="1badc-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="1badc-123">**Rapoarte**</span><span class="sxs-lookup"><span data-stu-id="1badc-123">**Reports**</span></span>
  
- <span data-ttu-id="1badc-124">Obțineți informații sensibile despre date cu [rapoarteLE DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="1badc-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="1badc-125">A se vedea detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="1badc-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
