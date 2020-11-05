---
title: Facturarea prin e-mail Azure modernă
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922141"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="8c01d-102">Facturarea prin e-mail în Azure</span><span class="sxs-lookup"><span data-stu-id="8c01d-102">Email invoicing in Azure</span></span>

<span data-ttu-id="8c01d-103">Trebuie să aveți un proprietar sau un rol de colaborator în profilul de facturare sau în contul său de facturare pentru a actualiza preferința facturii sale de e-mail.</span><span class="sxs-lookup"><span data-stu-id="8c01d-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="8c01d-104">După ce ați optat, toți utilizatorii cu roluri de proprietar, colaborator, cititori și Manager de facturi într-un profil de facturare își vor primi factura prin e-mail.</span><span class="sxs-lookup"><span data-stu-id="8c01d-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="8c01d-105">Conectați-vă la [portalul Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8c01d-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8c01d-106">Căutați **gestionarea costurilor + facturare**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8c01d-107">Selectați **facturi** din partea stângă, apoi selectați factură de **e-mail** din partea de sus a paginii.</span><span class="sxs-lookup"><span data-stu-id="8c01d-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="8c01d-108">Dacă aveți mai multe profiluri de facturare, selectați un profil de facturare, apoi selectați **înscriere**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="8c01d-109">Selectați **Actualizare**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-109">Select **Update**.</span></span>
6. <span data-ttu-id="8c01d-110">Dacă aveți mai multe profiluri de facturare, selectați un profil de facturare, apoi selectați **înscriere**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="8c01d-111">Oferiți altor persoane acces la vizualizarea, descărcarea și plata facturilor atribuindu-le rolul de manager de factură pentru un profil de facturare MCA sau MPA.</span><span class="sxs-lookup"><span data-stu-id="8c01d-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="8c01d-112">Dacă ați optat pentru a obține factura prin e-mail, utilizatorii primesc facturi și în e-mail.</span><span class="sxs-lookup"><span data-stu-id="8c01d-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="8c01d-113">Conectați-vă la [portalul Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8c01d-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8c01d-114">Căutați **gestionarea costurilor + facturare**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="8c01d-115">Selectați **profiluri de facturare** din partea stângă.</span><span class="sxs-lookup"><span data-stu-id="8c01d-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="8c01d-116">Din lista profiluri de facturare, selectați un profil de facturare pentru care doriți să atribuiți un rol de manager de facturi.</span><span class="sxs-lookup"><span data-stu-id="8c01d-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="8c01d-117">Selectați **control Access (iam)** din partea stângă, apoi selectați **Adăugare** din partea de sus a paginii.</span><span class="sxs-lookup"><span data-stu-id="8c01d-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="8c01d-118">În lista verticală rol, selectați **Facturare Manager**.</span><span class="sxs-lookup"><span data-stu-id="8c01d-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="8c01d-119">Introduceți adresa de e-mail a utilizatorului pentru a oferi acces.</span><span class="sxs-lookup"><span data-stu-id="8c01d-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="8c01d-120">Selectați **Salvare** pentru a atribui rolul.</span><span class="sxs-lookup"><span data-stu-id="8c01d-120">Select **Save** to assign the role.</span></span>
