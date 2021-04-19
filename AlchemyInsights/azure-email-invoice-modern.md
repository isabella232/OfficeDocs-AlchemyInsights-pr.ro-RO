---
title: Invoicing modern Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820838"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="15abe-102">Email invoicing in Azure</span><span class="sxs-lookup"><span data-stu-id="15abe-102">Email invoicing in Azure</span></span>

<span data-ttu-id="15abe-103">Trebuie să aveți un proprietar sau un rol colaborator în profilul de facturare sau contul său de facturare pentru a actualiza preferința sa de factură prin e-mail.</span><span class="sxs-lookup"><span data-stu-id="15abe-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="15abe-104">După ce ați optat pentru aceasta, toți utilizatorii cu roluri de proprietar, colaborator, cititori și manager de facturi pe un profil de facturare vor primi factura prin e-mail.</span><span class="sxs-lookup"><span data-stu-id="15abe-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="15abe-105">Conectați-vă [la portalul Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="15abe-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="15abe-106">Căutare **Gestionare costuri + Facturare**.</span><span class="sxs-lookup"><span data-stu-id="15abe-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="15abe-107">Selectați **Facturi din** partea stângă, apoi selectați Trimiteți o factură **prin** e-mail din partea de sus a paginii.</span><span class="sxs-lookup"><span data-stu-id="15abe-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="15abe-108">Dacă aveți mai multe profiluri de facturare, selectați un profil de facturare, apoi **selectați Înscriere**.</span><span class="sxs-lookup"><span data-stu-id="15abe-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="15abe-109">Selectați **Actualizare**.</span><span class="sxs-lookup"><span data-stu-id="15abe-109">Select **Update**.</span></span>
6. <span data-ttu-id="15abe-110">Dacă aveți mai multe profiluri de facturare, selectați un profil de facturare, apoi **selectați Înscriere**.</span><span class="sxs-lookup"><span data-stu-id="15abe-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="15abe-111">Oferiți altor persoane acces pentru a vizualiza, a descărca și a plăti facturi, atribuiându-le rolul de manager de facturi pentru un profil de facturare MCA sau MPA.</span><span class="sxs-lookup"><span data-stu-id="15abe-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="15abe-112">Dacă ați optat pentru a primi factura prin e-mail, utilizatorii vor primi facturile și prin e-mail.</span><span class="sxs-lookup"><span data-stu-id="15abe-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="15abe-113">Conectați-vă [la portalul Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="15abe-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="15abe-114">Căutare **Gestionare costuri + Facturare**.</span><span class="sxs-lookup"><span data-stu-id="15abe-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="15abe-115">Selectați **Profiluri** de facturare din partea stângă.</span><span class="sxs-lookup"><span data-stu-id="15abe-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="15abe-116">Din lista de profiluri de facturare, selectați un profil de facturare pentru care doriți să atribuiți un rol de manager de facturi.</span><span class="sxs-lookup"><span data-stu-id="15abe-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="15abe-117">Selectați **Control acces (IAM)** din partea stângă, apoi **selectați Adăugare** din partea de sus a paginii.</span><span class="sxs-lookup"><span data-stu-id="15abe-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="15abe-118">În lista verticală Rol, selectați **Manager de facturi**.</span><span class="sxs-lookup"><span data-stu-id="15abe-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="15abe-119">Introduceți adresa de e-mail a utilizatorului pentru a oferi acces.</span><span class="sxs-lookup"><span data-stu-id="15abe-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="15abe-120">Selectați **Salvare** pentru a atribui rolul.</span><span class="sxs-lookup"><span data-stu-id="15abe-120">Select **Save** to assign the role.</span></span>
