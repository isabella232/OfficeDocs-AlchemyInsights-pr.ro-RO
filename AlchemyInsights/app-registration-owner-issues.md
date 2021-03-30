---
title: Probleme cu Proprietarul înregistrării aplicațiilor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405318"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="f0a1d-102">Probleme cu Proprietarul înregistrării aplicațiilor</span><span class="sxs-lookup"><span data-stu-id="f0a1d-102">App Registration Owner issues</span></span>

<span data-ttu-id="f0a1d-103">În cele ce urmează, metodele disponibile pentru adăugarea de directori ca proprietari pentru înregistrările aplicațiilor:</span><span class="sxs-lookup"><span data-stu-id="f0a1d-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="f0a1d-104">Utilizarea Modulului Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="f0a1d-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="f0a1d-105">Referință: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="f0a1d-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="f0a1d-106">Utilizarea Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="f0a1d-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="f0a1d-107">Referință: [proprietar al aplicației az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="f0a1d-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="f0a1d-108">Utilizarea MS Graph -</span><span class="sxs-lookup"><span data-stu-id="f0a1d-108">Using MS Graph -</span></span>

    <span data-ttu-id="f0a1d-109">Referință: [Adăugare proprietar - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="f0a1d-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="f0a1d-110">Utilizarea Portalului Azure AD - Navigați [la portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Înregistrarea aplicațiilor > Selectați-vă aplicația > proprietarii > Adăugați proprietari</span><span class="sxs-lookup"><span data-stu-id="f0a1d-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="f0a1d-111">**Nu puteți vizualiza aplicația blade pentru înregistrările aplicațiilor chiar dacă sunteți proprietarul aplicației?**</span><span class="sxs-lookup"><span data-stu-id="f0a1d-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="f0a1d-112">Proprietarul unei aplicații nu este un rol administrativ.</span><span class="sxs-lookup"><span data-stu-id="f0a1d-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="f0a1d-113">În cazul în care setarea Restricționați accesul la portalul de administrare [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) este activată, doar administratorul va putea vizualiza aplicațiile în portalul de înregistrare a aplicațiilor.</span><span class="sxs-lookup"><span data-stu-id="f0a1d-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="f0a1d-114">Pentru ca un proprietar să poată vedea aplicațiile, dezactivați această setare (Setați la NU) sau atribuiți rolul de administrator proprietarului doar pentru aplicația specifică.</span><span class="sxs-lookup"><span data-stu-id="f0a1d-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="f0a1d-115">Cu toate acestea, veți avea nevoie de o licență Azure AD Premium P2 și veți activa Gestionarea [identităților privilegiați.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="f0a1d-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
