---
title: Setup DKIM în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666276"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="381c2-102">Setup DKIM în Office 365</span><span class="sxs-lookup"><span data-stu-id="381c2-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="381c2-103">Instrucțiunile complete pentru configurarea DKIM pentru domenii particularizate în Office 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="381c2-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="381c2-104">Pentru **fiecare** domeniu particularizat, trebuie să creați **două** DKIM CNAME înregistrări la serviciul de găzduire DNS al domeniului (de obicei, Registratorul de domeniu).</span><span class="sxs-lookup"><span data-stu-id="381c2-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="381c2-105">De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări DKIM CNAME: două pentru contoso.com și două pentru fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="381c2-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="381c2-106">Înregistrările DKIM CNAME pentru **fiecare** domeniu particularizat utilizează următoarele formate:</span><span class="sxs-lookup"><span data-stu-id="381c2-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="381c2-107">**Nume gazdă**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="381c2-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="381c2-108">**Puncte la adresa sau valoare**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="381c2-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="381c2-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="381c2-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="381c2-110">**Nume gazdă**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="381c2-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="381c2-111">**Puncte la adresa sau valoare**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="381c2-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="381c2-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="381c2-112">**TTL**: 3600</span></span>

   <span data-ttu-id="381c2-113">\<DomainGUID\> este textul `.mail.protection.outlook.com` din stânga în înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, `contoso-com` pentru domeniul contoso.com).</span><span class="sxs-lookup"><span data-stu-id="381c2-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="381c2-114">\<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înscris pentru Office 365 (de exemplu, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="381c2-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="381c2-115">După ce ați creat înregistrările CNAME pentru domeniile particularizate, completați următoarele instrucțiuni:</span><span class="sxs-lookup"><span data-stu-id="381c2-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="381c2-116">R.</span><span class="sxs-lookup"><span data-stu-id="381c2-116">a.</span></span> <span data-ttu-id="381c2-117">[Conectați-vă la Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la serviciu sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="381c2-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="381c2-118">B.</span><span class="sxs-lookup"><span data-stu-id="381c2-118">b.</span></span> <span data-ttu-id="381c2-119">Selectați pictograma lansator de aplicații în stânga sus și alegeți **admin**.</span><span class="sxs-lookup"><span data-stu-id="381c2-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="381c2-120">C.</span><span class="sxs-lookup"><span data-stu-id="381c2-120">c.</span></span> <span data-ttu-id="381c2-121">În navigare din stânga jos, extindeți **admin** și alegeți **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="381c2-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="381c2-122">D.</span><span class="sxs-lookup"><span data-stu-id="381c2-122">d.</span></span> <span data-ttu-id="381c2-123">Du-te la **protecția** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="381c2-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="381c2-124">E.</span><span class="sxs-lookup"><span data-stu-id="381c2-124">e.</span></span> <span data-ttu-id="381c2-125">Selectați domeniul și apoi alegeți **activați** pentru **mesaje de sign-in pentru acest domeniu cu semnături DKIM**.</span><span class="sxs-lookup"><span data-stu-id="381c2-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="381c2-126">Repetați acest pas pentru fiecare domeniu particularizat.</span><span class="sxs-lookup"><span data-stu-id="381c2-126">Repeat this step for each custom domain.</span></span>
