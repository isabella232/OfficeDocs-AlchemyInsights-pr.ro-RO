---
title: Cum se adaugă și se gestionează pașii recomandați de administratori
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755847"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="3ae67-102">Cum se adaugă și se gestionează pașii recomandați de administratori</span><span class="sxs-lookup"><span data-stu-id="3ae67-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="3ae67-103">În funcție de Descrierea problemei, am găsit o soluție pentru dvs.</span><span class="sxs-lookup"><span data-stu-id="3ae67-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="3ae67-104">Majoritatea clienților au putut să își rezolve singuri problema după ce au urmărit documentația noastră.</span><span class="sxs-lookup"><span data-stu-id="3ae67-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="3ae67-105">**Editarea administratorului de abonament sau a co-administratorului**</span><span class="sxs-lookup"><span data-stu-id="3ae67-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="3ae67-106">Administratorul de cont poate edita ambele roluri, în timp ce administratorul abonamentului poate modifica doar co-administratorii din [portalul Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="3ae67-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="3ae67-107">Adăugarea sau modificarea administratorilor de abonament Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="3ae67-108">**Actualizați administratorul abonamentului sau Co-Administrator pentru abonamentele interne (DIFUZe)**</span><span class="sxs-lookup"><span data-stu-id="3ae67-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="3ae67-109">Administratorul serviciului sau coadministratorul poate să servească automat această acțiune, utilizând următorii pași:</span><span class="sxs-lookup"><span data-stu-id="3ae67-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="3ae67-110">Conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) și faceți clic pe **gestionare costuri + facturare** în lama din stânga.</span><span class="sxs-lookup"><span data-stu-id="3ae67-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="3ae67-111">Faceți clic pe elementul linie cu abonamentul dvs.</span><span class="sxs-lookup"><span data-stu-id="3ae67-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="3ae67-112">Aceasta deschide prezentarea generală a abonamentului dumneavoastră.</span><span class="sxs-lookup"><span data-stu-id="3ae67-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="3ae67-113">Pe lama **abonamentului** , faceți clic pe **Proprietăți**.</span><span class="sxs-lookup"><span data-stu-id="3ae67-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="3ae67-114">Faceți clic pe butonul **administrator serviciu** .</span><span class="sxs-lookup"><span data-stu-id="3ae67-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="3ae67-115">Introduceți adresa de e-mail a utilizatorului pe care doriți să-l setați ca administrator de serviciu și faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ae67-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="3ae67-116">**Adăugare/Modificare/Eliminare co-administrator**</span><span class="sxs-lookup"><span data-stu-id="3ae67-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="3ae67-117">Conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) ca administrator de serviciu.</span><span class="sxs-lookup"><span data-stu-id="3ae67-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="3ae67-118">Deschideți [abonamente](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) și selectați un abonament.</span><span class="sxs-lookup"><span data-stu-id="3ae67-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="3ae67-119">(Co-adminstrators poate fi atribuită doar în domeniul abonamentului.)</span><span class="sxs-lookup"><span data-stu-id="3ae67-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="3ae67-120">Navigarea la administratorii Classic **Access Control (iam)**  >    >  **Adăugare**  >  **Adăugare co-administrator** pentru a deschide panoul **Adăugare co-** administrator (dacă opțiunea Adăugare co-administrator este dezactivată, aceasta denotă faptul că nu aveți permisiuni).</span><span class="sxs-lookup"><span data-stu-id="3ae67-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="3ae67-121">Selectați utilizatorul pe care doriți să-l adăugați și faceți clic pe **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="3ae67-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="3ae67-122">**află mai multe:**</span><span class="sxs-lookup"><span data-stu-id="3ae67-122">**Learn more:**</span></span>
- [<span data-ttu-id="3ae67-123">Adăugarea unui co-administrator</span><span class="sxs-lookup"><span data-stu-id="3ae67-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3ae67-124">Eliminarea unui co-administrator</span><span class="sxs-lookup"><span data-stu-id="3ae67-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3ae67-125">Modificarea administratorului serviciului</span><span class="sxs-lookup"><span data-stu-id="3ae67-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3ae67-126">Vizualizați Administratorul contului</span><span class="sxs-lookup"><span data-stu-id="3ae67-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3ae67-127">Gestionarea accesului utilizând RBAC și portalul Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="3ae67-128">**Adăugarea/ștergerea utilizatorilor utilizând Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="3ae67-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="3ae67-129">Puteți să adăugați utilizatori noi sau să ștergeți utilizatori existenți din organizația Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="3ae67-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="3ae67-130">Pentru a adăuga un utilizator nou, conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) ca administrator de utilizator al organizației.</span><span class="sxs-lookup"><span data-stu-id="3ae67-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="3ae67-131">Selectați **Azure Active Directory**, selectați **utilizatori** , apoi faceți clic pe **utilizator nou**.</span><span class="sxs-lookup"><span data-stu-id="3ae67-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="3ae67-132">În pagina **utilizator** , completați informațiile necesare.</span><span class="sxs-lookup"><span data-stu-id="3ae67-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="3ae67-133">Faceți clic pe **Creare**.</span><span class="sxs-lookup"><span data-stu-id="3ae67-133">Click **Create**.</span></span> <span data-ttu-id="3ae67-134">Utilizatorul este creat și adăugat la entitatea găzduită Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ae67-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="3ae67-135">**Aflați mai multe**:</span><span class="sxs-lookup"><span data-stu-id="3ae67-135">**Learn more**:</span></span>

- [<span data-ttu-id="3ae67-136">Adăugarea unui utilizator nou</span><span class="sxs-lookup"><span data-stu-id="3ae67-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3ae67-137">Ștergerea unui utilizator</span><span class="sxs-lookup"><span data-stu-id="3ae67-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3ae67-138">Adăugarea sau actualizarea informațiilor de profil ale unui utilizator utilizând Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3ae67-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="3ae67-139">**Documente recomandate**</span><span class="sxs-lookup"><span data-stu-id="3ae67-139">**Recommended documents**</span></span>

- [<span data-ttu-id="3ae67-140">Ce este controlul Access bazat pe roluri (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="3ae67-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="3ae67-141">Înțelegerea diferitelor roluri din Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="3ae67-142">Permisiuni pentru rolul de administrator în Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3ae67-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="3ae67-143">Tutorial: acordarea accesului pentru un utilizator utilizând RBAC și portalul Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="3ae67-144">Depanarea RBAC în Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="3ae67-145">Organizarea resurselor cu grupurile de gestionare Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="3ae67-146">Cum să solicitați o copie a facturii Azure prin e-mail</span><span class="sxs-lookup"><span data-stu-id="3ae67-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="3ae67-147">Cum să adăugați, să actualizați sau să eliminați un card de credit sau de debit din Azure</span><span class="sxs-lookup"><span data-stu-id="3ae67-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="3ae67-148">Abonament de gestionare (reactivare/anulare/comutare)</span><span class="sxs-lookup"><span data-stu-id="3ae67-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



