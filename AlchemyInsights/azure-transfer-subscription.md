---
title: Transferați proprietatea de facturare Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922167"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="c2101-102">Transferați proprietatea de facturare Azure</span><span class="sxs-lookup"><span data-stu-id="c2101-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="c2101-103">Conectați-vă la [portalul Azure](https://portal.azure.com/) ca administrator al contului de facturare care are abonamentul pe care doriți să-l transferați.</span><span class="sxs-lookup"><span data-stu-id="c2101-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="c2101-104">Dacă nu sunteți sigur dacă sunteți și administrator sau dacă trebuie să determinați cine este, consultați [determinarea administratorului de facturare a contului](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="c2101-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="c2101-105">Căutați în **gestionarea costurilor + facturare**.</span><span class="sxs-lookup"><span data-stu-id="c2101-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="c2101-106">Selectați **abonamente** din panoul din stânga.</span><span class="sxs-lookup"><span data-stu-id="c2101-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="c2101-107">În funcție de Access, poate fi necesar să selectați un domeniu de facturare, apoi **abonamente** sau **abonamente Azure**.</span><span class="sxs-lookup"><span data-stu-id="c2101-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="c2101-108">Selectați **transferați proprietatea de facturare** pentru abonamentul pe care doriți să-l transferați</span><span class="sxs-lookup"><span data-stu-id="c2101-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="c2101-109">Introduceți adresa de e-mail a unui utilizator care este administrator de facturare al contului care va fi noul proprietar pentru abonament, apoi selectați **Trimitere solicitare de transfer**</span><span class="sxs-lookup"><span data-stu-id="c2101-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="c2101-110">Utilizatorul primește un e-mail cu instrucțiuni pentru a revizui solicitarea de transfer.</span><span class="sxs-lookup"><span data-stu-id="c2101-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="c2101-111">Pentru a aproba solicitarea de transfer, utilizatorul selectează linkul din e-mail și urmează instrucțiunile.</span><span class="sxs-lookup"><span data-stu-id="c2101-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="c2101-112">**Notă** : dacă transferați proprietatea de facturare a abonamentului la un cont de utilizator într-o altă entitate găzduită Azure AD [, toate](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)atribuirile pentru gestionarea resurselor din abonament sunt eliminate definitiv.</span><span class="sxs-lookup"><span data-stu-id="c2101-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="c2101-113">Doar noul proprietar va avea acces la gestionarea resurselor din abonament.</span><span class="sxs-lookup"><span data-stu-id="c2101-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="c2101-114">Pentru mai multe informații, consultați [transferul abonamentului la un utilizator într-o altă entitate găzduită AZURE AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c2101-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c2101-115">**Documente recomandate**</span><span class="sxs-lookup"><span data-stu-id="c2101-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="c2101-116">Transferați proprietatea de facturare a unui abonament Azure în alt cont</span><span class="sxs-lookup"><span data-stu-id="c2101-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="c2101-117">Despre transferul proprietății de facturare pentru un abonament Azure</span><span class="sxs-lookup"><span data-stu-id="c2101-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="c2101-118">Transferați Visual Studio, Microsoft Partner Network (MPN) și plătiți pe măsură ce accesați abonamente Dev/test</span><span class="sxs-lookup"><span data-stu-id="c2101-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="c2101-119">Întrebări frecvente despre proprietatea transfer</span><span class="sxs-lookup"><span data-stu-id="c2101-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="c2101-120">Depanarea problemelor legate de proprietatea transfer</span><span class="sxs-lookup"><span data-stu-id="c2101-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
