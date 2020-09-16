---
title: Crearea politicilor de etichetare AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732187"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="7490a-102">Crearea politicilor de etichetare AIP</span><span class="sxs-lookup"><span data-stu-id="7490a-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="7490a-103">Etichetele Azure Information Protection (AIP) pot fi utilizate cu întreaga gamă de date pe care o organizație le creează și le stochează, de obicei, de la cea mai mică clasificare a datelor personale, la cea mai înaltă clasificare a datelor foarte confidențiale.</span><span class="sxs-lookup"><span data-stu-id="7490a-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="7490a-104">Politicile de protecție a informațiilor Azure se aplică pentru clientul Classic Azure Information Protection (AIP), nu pentru  [clientul de etichetare unificată AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="7490a-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="7490a-105">Puteți configura mai multe elemente într-o politică AIP, inclusiv opțiuni, cum ar fi:</span><span class="sxs-lookup"><span data-stu-id="7490a-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="7490a-106">Opțiunea pentru care etichetă va permite administratorilor sau documentelor și e-mailurilor de clasificare și protecție (opțional) pentru utilizatori</span><span class="sxs-lookup"><span data-stu-id="7490a-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="7490a-107">Opțiunea de a impune clasificarea atunci când utilizatorii salvează documente și trimit mesaje de e-mail</span><span class="sxs-lookup"><span data-stu-id="7490a-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="7490a-108">Opțiunea de a eticheta automat un mesaj de e-mail, pe baza atașărilor sale.</span><span class="sxs-lookup"><span data-stu-id="7490a-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="7490a-109">Opțiunea de a controla dacă bara de protecție a informațiilor se afișează în aplicațiile Office</span><span class="sxs-lookup"><span data-stu-id="7490a-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="7490a-110">Pentru opțiuni suplimentare și informații despre politicile de protecție a informațiilor Azure, consultați: [Prezentare generală a politicii de protecție a informațiilor Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="7490a-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="7490a-111">Pentru alte resurse utile în ceea ce privește politicile AIP, consultați:</span><span class="sxs-lookup"><span data-stu-id="7490a-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="7490a-112">Tutorial: Configurarea setărilor politicii de protecție a informațiilor Azure și crearea unei etichete noi</span><span class="sxs-lookup"><span data-stu-id="7490a-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7490a-113">Configurarea politicii de protecție a informațiilor Azure</span><span class="sxs-lookup"><span data-stu-id="7490a-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="7490a-114">Crearea și configurarea etichetelor de sensibilitate și a politicilor acestora</span><span class="sxs-lookup"><span data-stu-id="7490a-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="7490a-115">Ghiduri introductive pentru scenariile obișnuite care utilizează Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7490a-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="7490a-116">Revizuirea documentației Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7490a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="7490a-117">Cerințe pentru protecția informațiilor Azure</span><span class="sxs-lookup"><span data-stu-id="7490a-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="7490a-118">Tutorial de pornire rapidă pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7490a-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7490a-119">Descărcați clientul Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7490a-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)