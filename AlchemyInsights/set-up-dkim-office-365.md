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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509396"
---
# <a name="setup-dkim"></a><span data-ttu-id="906a5-102">Configurare DKIM</span><span class="sxs-lookup"><span data-stu-id="906a5-102">Setup DKIM</span></span>

<span data-ttu-id="906a5-103">Instrucțiunicomplete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="906a5-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="906a5-104">Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări DKIM CNAME la serviciul de găzduire DNS al domeniului (de obicei, registratorul de domeniu).</span><span class="sxs-lookup"><span data-stu-id="906a5-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="906a5-105">De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="906a5-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="906a5-106">Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:</span><span class="sxs-lookup"><span data-stu-id="906a5-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="906a5-107">**Nume gazdă**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="906a5-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="906a5-108">**Puncte de adresă sau valoare:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="906a5-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="906a5-109">**TTL**: 3600 (</span><span class="sxs-lookup"><span data-stu-id="906a5-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="906a5-110">**Nume gazdă**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="906a5-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="906a5-111">**Puncte de adresă sau valoare:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="906a5-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="906a5-112">**TTL**: 3600 (</span><span class="sxs-lookup"><span data-stu-id="906a5-112">**TTL**: 3600</span></span>

   <span data-ttu-id="906a5-113">\<DomainGUID\>este textul din stânga `.mail.protection.outlook.com` înregistrării MX particularizate pentru domeniul particularizat (de exemplu, `contoso-com` pentru contoso.com de domeniu).</span><span class="sxs-lookup"><span data-stu-id="906a5-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="906a5-114">\<InitialDomain\>este domeniul pe care l-ați utilizat atunci când v-ați înscris la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="906a5-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="906a5-115">După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:</span><span class="sxs-lookup"><span data-stu-id="906a5-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="906a5-116">R.</span><span class="sxs-lookup"><span data-stu-id="906a5-116">a.</span></span> <span data-ttu-id="906a5-117">[conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="906a5-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="906a5-118">B.</span><span class="sxs-lookup"><span data-stu-id="906a5-118">b.</span></span> <span data-ttu-id="906a5-119">Selectați pictograma lansator de aplicații din stânga sus și alegeți **Admin**.</span><span class="sxs-lookup"><span data-stu-id="906a5-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="906a5-120">C.</span><span class="sxs-lookup"><span data-stu-id="906a5-120">c.</span></span> <span data-ttu-id="906a5-121">În navigarea din stânga jos, extindeți **Admin** și alegeți **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="906a5-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="906a5-122">D.</span><span class="sxs-lookup"><span data-stu-id="906a5-122">d.</span></span> <span data-ttu-id="906a5-123">Du-te la **Protecție**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="906a5-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="906a5-124">E.</span><span class="sxs-lookup"><span data-stu-id="906a5-124">e.</span></span> <span data-ttu-id="906a5-125">Selectați domeniul, apoi **alegeți Activare** pentru **Semnare mesaje pentru acest domeniu cu semnături DKIM**.</span><span class="sxs-lookup"><span data-stu-id="906a5-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="906a5-126">Repetați acest pas pentru fiecare domeniu particularizat.</span><span class="sxs-lookup"><span data-stu-id="906a5-126">Repeat this step for each custom domain.</span></span>
