---
title: DKIM de configurare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808719"
---
# <a name="setup-dkim"></a><span data-ttu-id="b580a-102">DKIM de configurare</span><span class="sxs-lookup"><span data-stu-id="b580a-102">Setup DKIM</span></span>

<span data-ttu-id="b580a-103">Instrucțiunile complete pentru configurarea DKIM pentru domenii particularizate în Microsoft 365 sunt [aici](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="b580a-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="b580a-104">Pentru **fiecare** domeniu particularizat, trebuie să creați **două** înregistrări CNAME DKIM la serviciul de găzduire DNS al domeniului (de obicei, Registratorul de domeniu).</span><span class="sxs-lookup"><span data-stu-id="b580a-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="b580a-105">De exemplu, contoso.com și fourthcoffee.com necesită patru înregistrări CNAME DKIM: două pentru contoso.com și două pentru fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="b580a-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="b580a-106">Înregistrările CNAME DKIM pentru **fiecare** domeniu particularizat utilizează următoarele formate:</span><span class="sxs-lookup"><span data-stu-id="b580a-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="b580a-107">**Nume gazdă**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b580a-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b580a-108">**Indică adresa sau valoarea**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b580a-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b580a-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b580a-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="b580a-110">**Nume gazdă**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="b580a-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="b580a-111">**Indică adresa sau valoarea**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="b580a-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="b580a-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="b580a-112">**TTL**: 3600</span></span>

   <span data-ttu-id="b580a-113">\<DomainGUID\> este textul de la stânga `.mail.protection.outlook.com` în înregistrarea MX particularizată pentru domeniul particularizat (de exemplu, `contoso-com` pentru domeniul contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b580a-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="b580a-114">\<InitialDomain\> este domeniul pe care l-ați utilizat atunci când v-ați înregistrat la Microsoft 365 (de exemplu, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="b580a-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="b580a-115">După ce ați creat înregistrările CNAME pentru domeniile particularizate, parcurgeți următoarele instrucțiuni:</span><span class="sxs-lookup"><span data-stu-id="b580a-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="b580a-116">un.</span><span class="sxs-lookup"><span data-stu-id="b580a-116">a.</span></span> <span data-ttu-id="b580a-117">[Conectați-vă la Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul de la locul de muncă sau de la școală.</span><span class="sxs-lookup"><span data-stu-id="b580a-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="b580a-118">b.</span><span class="sxs-lookup"><span data-stu-id="b580a-118">b.</span></span> <span data-ttu-id="b580a-119">Selectați pictograma lansator de aplicații din partea stângă sus și alegeți **administrator**.</span><span class="sxs-lookup"><span data-stu-id="b580a-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="b580a-120">c.</span><span class="sxs-lookup"><span data-stu-id="b580a-120">c.</span></span> <span data-ttu-id="b580a-121">În navigarea din stânga jos, extindeți **administratorul** și alegeți **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b580a-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="b580a-122">d.</span><span class="sxs-lookup"><span data-stu-id="b580a-122">d.</span></span> <span data-ttu-id="b580a-123">Accesați DKIM de **protecție**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b580a-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="b580a-124">e.</span><span class="sxs-lookup"><span data-stu-id="b580a-124">e.</span></span> <span data-ttu-id="b580a-125">Selectați domeniul, apoi alegeți **Activare** pentru **semnați mesaje pentru acest domeniu cu semnături DKIM**.</span><span class="sxs-lookup"><span data-stu-id="b580a-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="b580a-126">Repetați acest pas pentru fiecare domeniu particularizat.</span><span class="sxs-lookup"><span data-stu-id="b580a-126">Repeat this step for each custom domain.</span></span>
