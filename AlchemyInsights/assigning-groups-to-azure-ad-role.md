---
title: Atribuirea grupurilor la rolul Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885395"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="d2239-102">Atribuirea grupurilor la rolul Azure AD</span><span class="sxs-lookup"><span data-stu-id="d2239-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="d2239-103">Pentru a atribui un grup de anunțuri Azure cu sursă de autoritate în Azure AD la un rol de publicitate Azure, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="d2239-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="d2239-104">Creați un grup nou-pentru a crea un grup nou:</span><span class="sxs-lookup"><span data-stu-id="d2239-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="d2239-105">un.</span><span class="sxs-lookup"><span data-stu-id="d2239-105">a.</span></span> <span data-ttu-id="d2239-106">Conectați-vă la centrul de administrare Azure AD cu **administrator de rol privilegiat** sau permisiuni de **administrator global** .</span><span class="sxs-lookup"><span data-stu-id="d2239-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="d2239-107">b.</span><span class="sxs-lookup"><span data-stu-id="d2239-107">b.</span></span> <span data-ttu-id="d2239-108">Selectați **grupuri Azure Active Directory > > toate grupurile > grup nou**.</span><span class="sxs-lookup"><span data-stu-id="d2239-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="d2239-109">c.</span><span class="sxs-lookup"><span data-stu-id="d2239-109">c.</span></span> <span data-ttu-id="d2239-110">Creați grupul.</span><span class="sxs-lookup"><span data-stu-id="d2239-110">Create the group.</span></span>

2. <span data-ttu-id="d2239-111">Atribuiți rolul grupului fie în timpul creării grupului, fie după crearea grupului.</span><span class="sxs-lookup"><span data-stu-id="d2239-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="d2239-112">un.</span><span class="sxs-lookup"><span data-stu-id="d2239-112">a.</span></span> <span data-ttu-id="d2239-113">Pentru a atribui un rol grupului în momentul creării unui grup, comutați la grupul se **pot atribui rolurile** de returnare Azure AD și puteți crea grupul.</span><span class="sxs-lookup"><span data-stu-id="d2239-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="d2239-114">b.</span><span class="sxs-lookup"><span data-stu-id="d2239-114">b.</span></span> <span data-ttu-id="d2239-115">Pentru a atribui un rol grupului după ce a fost creat, navigați la fila **roluri atribuite** pentru grupul nou creat și atribuiți rolul grupului.</span><span class="sxs-lookup"><span data-stu-id="d2239-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="d2239-116">**Gestionarea apartenenței la un grup căruia i se atribuie rolul Azure AD**</span><span class="sxs-lookup"><span data-stu-id="d2239-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="d2239-117">Pentru a împiedica elevația privilegiilor, în mod implicit, doar administratorii de rol privilegiat și administratorii globali pot modifica apartenența la un grup atribuit unui rol.</span><span class="sxs-lookup"><span data-stu-id="d2239-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="d2239-118">Cu toate acestea, pot alege să atribuie un proprietar unui astfel de grup și să delege această activitate.</span><span class="sxs-lookup"><span data-stu-id="d2239-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="d2239-119">Pentru mai multe detalii despre atribuirea grupurilor nor la roluri Azure AD, consultați [atribuirea unui rol de publicitate în grupul Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="d2239-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="d2239-120">Pentru mai multe detalii despre depanarea rolurilor atribuite grupurilor Cloud, consultați [Depanarea rolurilor atribuite grupurilor Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="d2239-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





