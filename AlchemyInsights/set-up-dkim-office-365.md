---
title: Configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645684"
---
# <a name="setup-dkim"></a><span data-ttu-id="466be-102">Configurare DKIM</span><span class="sxs-lookup"><span data-stu-id="466be-102">Setup DKIM</span></span>

<span data-ttu-id="466be-103">Instrucțiunicomplete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="466be-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="466be-104">Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări DKIM CNAME la serviciul de găzduire DNS al domeniului (de obicei, registratorul de domeniu).</span><span class="sxs-lookup"><span data-stu-id="466be-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="466be-105">De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="466be-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="466be-106">Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:</span><span class="sxs-lookup"><span data-stu-id="466be-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="466be-107">**Nume gazdă**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="466be-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="466be-108">**Puncte de adresă sau valoare:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="466be-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="466be-109">**TTL**: 3600 (</span><span class="sxs-lookup"><span data-stu-id="466be-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="466be-110">**Nume gazdă**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="466be-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="466be-111">**Puncte de adresă sau valoare:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="466be-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="466be-112">**TTL**: 3600 (</span><span class="sxs-lookup"><span data-stu-id="466be-112">**TTL**: 3600</span></span>

   <span data-ttu-id="466be-113">\<DomainGUID\> este textul din `.mail.protection.outlook.com` stânga înregistrării MX particularizate pentru domeniul `contoso-com` particularizat (de exemplu, pentru contoso.com de domeniu).</span><span class="sxs-lookup"><span data-stu-id="466be-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="466be-114">\<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înscris la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="466be-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="466be-115">După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:</span><span class="sxs-lookup"><span data-stu-id="466be-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="466be-116">R.</span><span class="sxs-lookup"><span data-stu-id="466be-116">a.</span></span> <span data-ttu-id="466be-117">[conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="466be-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="466be-118">B.</span><span class="sxs-lookup"><span data-stu-id="466be-118">b.</span></span> <span data-ttu-id="466be-119">Selectați pictograma lansator de aplicații din stânga sus și alegeți **Admin**.</span><span class="sxs-lookup"><span data-stu-id="466be-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="466be-120">C.</span><span class="sxs-lookup"><span data-stu-id="466be-120">c.</span></span> <span data-ttu-id="466be-121">În navigarea din stânga jos, extindeți **Admin** și alegeți **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="466be-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="466be-122">D.</span><span class="sxs-lookup"><span data-stu-id="466be-122">d.</span></span> <span data-ttu-id="466be-123">Du-te la **Protecție** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="466be-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="466be-124">E.</span><span class="sxs-lookup"><span data-stu-id="466be-124">e.</span></span> <span data-ttu-id="466be-125">Selectați domeniul, apoi **alegeți Activare** pentru **Semnare mesaje pentru acest domeniu cu semnături DKIM**.</span><span class="sxs-lookup"><span data-stu-id="466be-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="466be-126">Repetați acest pas pentru fiecare domeniu particularizat.</span><span class="sxs-lookup"><span data-stu-id="466be-126">Repeat this step for each custom domain.</span></span>
