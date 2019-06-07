---
title: Configurare DKIM în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765341"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="f41e1-102">Configurare DKIM în Office 365</span><span class="sxs-lookup"><span data-stu-id="f41e1-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="f41e1-103">Instrucţiuni complete pentru configurarea DKIM pentru domenii particularizate în Office 365 sunt [aici](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f41e1-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="f41e1-104">Pentru **fiecare** domeniu personalizat, trebuie să creaţi **două** înregistrări DKIM CNAME la serviciul găzduire DNS al domeniului (de obicei, Registratorul de domeniu).</span><span class="sxs-lookup"><span data-stu-id="f41e1-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="f41e1-105">De exemplu, contoso.com şi fourthcoffee.com necesită patru DKIM CNAME records: două pentru contoso.com şi două pentru fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="f41e1-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="f41e1-106">Înregistrările DKIM CNAME pentru **fiecare** domeniu personalizat utilizează următoarele formate:</span><span class="sxs-lookup"><span data-stu-id="f41e1-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="f41e1-107">**Nume gazdă**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f41e1-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f41e1-108">**Puncte la adresa sau valoare**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f41e1-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f41e1-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f41e1-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="f41e1-110">**Nume gazdă**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="f41e1-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="f41e1-111">**Puncte la adresa sau valoare**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="f41e1-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="f41e1-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="f41e1-112">**TTL**: 3600</span></span>

   <span data-ttu-id="f41e1-113">\<DomainGUID\> este textul din stanga `.mail.protection.outlook.com` în personalizate înregistrarea MX pentru domeniul personalizate (de exemplu, `contoso-com` pentru domeniul contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f41e1-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="f41e1-114">\<InitialDomain\> este un domeniu de aţi folosit atunci când v-aţi înscris pentru Office 365 (de exemplu, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="f41e1-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="f41e1-115">După ce aţi creat înregistrări CNAME pentru domenii particularizate, completaţi următoarele instrucţiuni:</span><span class="sxs-lookup"><span data-stu-id="f41e1-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="f41e1-116">un.</span><span class="sxs-lookup"><span data-stu-id="f41e1-116">a.</span></span> <span data-ttu-id="f41e1-117">[Conectaţi-vă la Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) cu contul dvs de lucru sau şcoală.</span><span class="sxs-lookup"><span data-stu-id="f41e1-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="f41e1-118">b.</span><span class="sxs-lookup"><span data-stu-id="f41e1-118">b.</span></span> <span data-ttu-id="f41e1-119">Selectaţi pictograma app lansator din stânga şi selectaţi **Admin**.</span><span class="sxs-lookup"><span data-stu-id="f41e1-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="f41e1-120">c.</span><span class="sxs-lookup"><span data-stu-id="f41e1-120">c.</span></span> <span data-ttu-id="f41e1-121">În stânga de navigare, extindeţi **Admin** şi alege **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f41e1-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="f41e1-122">d.</span><span class="sxs-lookup"><span data-stu-id="f41e1-122">d.</span></span> <span data-ttu-id="f41e1-123">Du-te la **protectia** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="f41e1-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="f41e1-124">e.</span><span class="sxs-lookup"><span data-stu-id="f41e1-124">e.</span></span> <span data-ttu-id="f41e1-125">Selectaţi domeniul şi apoi **permite** pentru **semn mesaje pentru acest domeniu, cu semnăturile de DKIM**.</span><span class="sxs-lookup"><span data-stu-id="f41e1-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="f41e1-126">Repetaţi acest pas pentru fiecare domeniu particularizat.</span><span class="sxs-lookup"><span data-stu-id="f41e1-126">Repeat this step for each custom domain.</span></span>
