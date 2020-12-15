---
title: Activați gestionarea costurilor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678769"
---
# <a name="enable-cost-management"></a><span data-ttu-id="fa031-102">Activați gestionarea costurilor</span><span class="sxs-lookup"><span data-stu-id="fa031-102">Enable cost management</span></span>

<span data-ttu-id="fa031-103">**Ce înseamnă "costurile sunt dezactivate pentru organizația dvs."?**</span><span class="sxs-lookup"><span data-stu-id="fa031-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="fa031-104">Organizațiile care utilizează conturi Enterprise Agreement (EA) sau Microsoft Customer Agreement (MCA) pot dezactiva accesul la informații despre costuri și informații despre prețuri.</span><span class="sxs-lookup"><span data-stu-id="fa031-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="fa031-105">După ce vă conectați la Azure portal, aceștia pot utiliza API-urile de facturare pentru a obține programatic facturi (după ce ați optat) și detalii de utilizare.</span><span class="sxs-lookup"><span data-stu-id="fa031-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="fa031-106">**Cum se permite utilizatorilor suplimentari să acceseze facturi**</span><span class="sxs-lookup"><span data-stu-id="fa031-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="fa031-107">Accesați **Blade abonamente** în Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fa031-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fa031-108">Selectați **facturi** , apoi **acces la facturi**.</span><span class="sxs-lookup"><span data-stu-id="fa031-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="fa031-109">Activați accesul, urmat salvând modificările, pentru a le permite utilizatorilor din rolurile de domeniu de abonament să descarce facturi.</span><span class="sxs-lookup"><span data-stu-id="fa031-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="fa031-110">Administratorul de cont poate configura, de asemenea, să aibă facturile trimise prin e-mail.</span><span class="sxs-lookup"><span data-stu-id="fa031-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="fa031-111">Pentru a afla mai multe, consultați [obținerea facturii prin e-mail](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="fa031-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="fa031-112">**Cum se adaugă utilizatori la rolul de cititor de facturare**</span><span class="sxs-lookup"><span data-stu-id="fa031-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="fa031-113">Accesați **Blade abonamente** în Azure portal.</span><span class="sxs-lookup"><span data-stu-id="fa031-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="fa031-114">Selectați **control Access (iam)** , apoi faceți clic pe **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="fa031-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="fa031-115">Alegeți **cititor de facturare** în pagina **Selectați un rol** .</span><span class="sxs-lookup"><span data-stu-id="fa031-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="fa031-116">Tastați mesajul de e-mail al utilizatorului pe care doriți să-l invitați, apoi faceți clic pe **OK** pentru a trimite invitația.</span><span class="sxs-lookup"><span data-stu-id="fa031-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="fa031-117">Urmați instrucțiunile furnizate în mesajul de e-mail invitație pentru a vă conecta ca cititor de facturare.</span><span class="sxs-lookup"><span data-stu-id="fa031-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="fa031-118">Pentru mai multe informații, consultați [acordarea accesului la facturare](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="fa031-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="fa031-119">**Documente recomandate**</span><span class="sxs-lookup"><span data-stu-id="fa031-119">**Recommended documents**</span></span>

- [<span data-ttu-id="fa031-120">Activarea vizualizărilor DA și AO prin portalul EA</span><span class="sxs-lookup"><span data-stu-id="fa031-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="fa031-121">Costurile incluse în gestionarea costurilor</span><span class="sxs-lookup"><span data-stu-id="fa031-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="fa031-122">Oferte acceptate Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="fa031-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="fa031-123">Revizuirea costurilor din analiza costurilor</span><span class="sxs-lookup"><span data-stu-id="fa031-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="fa031-124">Furnizarea accesului la informațiile de facturare</span><span class="sxs-lookup"><span data-stu-id="fa031-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="fa031-125">Verificarea accesului la un contract de client Microsoft</span><span class="sxs-lookup"><span data-stu-id="fa031-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






