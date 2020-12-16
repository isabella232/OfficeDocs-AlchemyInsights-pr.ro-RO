---
title: Transfer servicii-mutați toate serviciile RDFE la un alt abonament
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692174"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="bd991-102">Transfer servicii-mutați toate serviciile RDFE la un alt abonament</span><span class="sxs-lookup"><span data-stu-id="bd991-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="bd991-103">**Mutarea resurselor**</span><span class="sxs-lookup"><span data-stu-id="bd991-103">**Move resources**</span></span>

<span data-ttu-id="bd991-104">Resursele Azure pot fi mutate la un alt abonament Azure sau la un grup de resurse sub același abonament utilizând Azure portal, Azure PowerShell, Azure CLI sau REST API pentru a muta resursele.</span><span class="sxs-lookup"><span data-stu-id="bd991-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="bd991-105">Înainte de a putea muta resursele, consultați:</span><span class="sxs-lookup"><span data-stu-id="bd991-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="bd991-106">Listă de verificare înainte de mutarea resurselor</span><span class="sxs-lookup"><span data-stu-id="bd991-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="bd991-107">Servicii care pot fi mutate</span><span class="sxs-lookup"><span data-stu-id="bd991-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bd991-108">Cum se validează mutarea</span><span class="sxs-lookup"><span data-stu-id="bd991-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="bd991-109">Mutarea ghidării pentru servicii</span><span class="sxs-lookup"><span data-stu-id="bd991-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="bd991-110">Pentru a muta resursele existente într-un alt grup de resurse sau abonament, puteți utiliza:</span><span class="sxs-lookup"><span data-stu-id="bd991-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="bd991-111">Portalul Azure</span><span class="sxs-lookup"><span data-stu-id="bd991-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="bd991-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd991-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="bd991-113">CLI Azure</span><span class="sxs-lookup"><span data-stu-id="bd991-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="bd991-114">API REST</span><span class="sxs-lookup"><span data-stu-id="bd991-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="bd991-115">Tutorial: [mutați resursele Azure într-un alt grup de resurse sau abonament](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="bd991-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="bd991-116">**Depanarea erorilor cu Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="bd991-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="bd991-117">Consultați articolele de mai jos pentru a afla despre unele erori comune de implementare Azure și a primi informații pentru a le rezolva.</span><span class="sxs-lookup"><span data-stu-id="bd991-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="bd991-118">Dacă nu găsiți codul de eroare pentru eroarea de implementare, consultați [Găsirea codului de eroare](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="bd991-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="bd991-119">Depanarea erorilor de implementare</span><span class="sxs-lookup"><span data-stu-id="bd991-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="bd991-120">Depanarea mutării resurselor Azure în grup de resurse noi sau abonament</span><span class="sxs-lookup"><span data-stu-id="bd991-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="bd991-121">Rețineți că, dacă doriți să faceți upgrade abonamentului Azure, cum ar fi trecerea de la gratuit la plată-ca-Go, va trebui să efectuați conversia abonamentului.</span><span class="sxs-lookup"><span data-stu-id="bd991-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="bd991-122">Pentru a face upgrade la o versiune de încercare gratuită, consultați [upgrade-ul versiunii de încercare gratuite sau Microsoft imaginați-vă abonamentul Azure la plată-ca-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="bd991-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="bd991-123">Pentru a modifica un cont pay-as-Go, consultați [Modificarea abonamentului Azure pay-as-Go la o altă ofertă](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="bd991-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="bd991-124">**Pentru a adăuga sau a asocia un abonament Azure la entitatea găzduită Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="bd991-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="bd991-125">Conectați-vă și selectați abonamentul pe care doriți să-l utilizați din [pagina Abonamente din Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="bd991-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="bd991-126">Selectați **Modificați directorul**.</span><span class="sxs-lookup"><span data-stu-id="bd991-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="bd991-127">Revizuiți avertismentele care apar, apoi selectați **modificare**.</span><span class="sxs-lookup"><span data-stu-id="bd991-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="bd991-128">Directorul este modificat pentru abonament și veți primi un mesaj de succes.</span><span class="sxs-lookup"><span data-stu-id="bd991-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="bd991-129">Utilizați comutatorul *Director* pentru a merge la noul director.</span><span class="sxs-lookup"><span data-stu-id="bd991-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="bd991-130">Este posibil să dureze până la 10 minute pentru ca totul să se afișeze corect.</span><span class="sxs-lookup"><span data-stu-id="bd991-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="bd991-131">**Documente recomandate**</span><span class="sxs-lookup"><span data-stu-id="bd991-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="bd991-132">Transferul dreptului de proprietate asupra unui abonament Azure</span><span class="sxs-lookup"><span data-stu-id="bd991-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="bd991-133">Mutarea resurselor în grup de resurse sau abonament nou</span><span class="sxs-lookup"><span data-stu-id="bd991-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="bd991-134">Gestionarea resurselor utilizând Azure portal</span><span class="sxs-lookup"><span data-stu-id="bd991-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
