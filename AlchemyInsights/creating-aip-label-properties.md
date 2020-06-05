---
title: Crearea politicilor de etichete AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569509"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="ae490-102">Crearea politicilor de etichete AIP</span><span class="sxs-lookup"><span data-stu-id="ae490-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="ae490-103">Etichetele Azure Information Protection (AIP) pot fi utilizate cu întreaga gamă de date pe care o organizație le creează și stochează, de obicei, de la cea mai joasă clasificare a datelor cu caracter personal, la cea mai înaltă clasificare a datelor extrem de confidențiale.</span><span class="sxs-lookup"><span data-stu-id="ae490-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="ae490-104">Azure Information Protection Politici se aplică azure information protection(AIP) client clasic și nu [AIP unificat etichetarea client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="ae490-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="ae490-105">Puteți configura mai multe elemente într-o politică AIP, inclusiv opțiuni precum:</span><span class="sxs-lookup"><span data-stu-id="ae490-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="ae490-106">Opțiune pentru care eticheta va permite administratorilor sau utilizatorului să clasifice și să protecție (opțional) documente și e-mailuri</span><span class="sxs-lookup"><span data-stu-id="ae490-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="ae490-107">Opțiunea de a impune clasificarea atunci când utilizatorii salvează documente și trimit e-mailuri</span><span class="sxs-lookup"><span data-stu-id="ae490-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="ae490-108">Opțiunea de a eticheta automat un mesaj de e-mail, pe baza atașărilor sale.</span><span class="sxs-lookup"><span data-stu-id="ae490-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="ae490-109">Opțiunea de a controla dacă bara de protecție a informațiilor este afișată în aplicațiile Office</span><span class="sxs-lookup"><span data-stu-id="ae490-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="ae490-110">Pentru opțiuni suplimentare și informații despre politicile azure privind protecția informațiilor, consultați: [Prezentare generală a politicii azure privind protecția informațiilor](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="ae490-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="ae490-111">Pentru alte resurse utile în ceea ce privește politicile AIP, consultați:</span><span class="sxs-lookup"><span data-stu-id="ae490-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="ae490-112">Tutorial: Configurarea setărilor de politică Azure Information Protection și crearea unei etichete noi</span><span class="sxs-lookup"><span data-stu-id="ae490-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ae490-113">Configurarea politicii Azure protecția informațiilor</span><span class="sxs-lookup"><span data-stu-id="ae490-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="ae490-114">Crearea și configurarea etichetelor de sensibilitate și a politicilor acestora</span><span class="sxs-lookup"><span data-stu-id="ae490-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="ae490-115">Ghiduri de utilizare pentru scenarii comune care utilizează Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="ae490-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="ae490-116">Examinați documentația Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="ae490-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="ae490-117">Cerințe pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="ae490-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="ae490-118">Tutorial de pornire rapidă pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="ae490-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="ae490-119">Descărcați clientul Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="ae490-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)