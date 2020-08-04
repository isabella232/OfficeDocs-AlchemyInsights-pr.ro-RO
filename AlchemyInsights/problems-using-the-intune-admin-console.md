---
title: Probleme la utilizarea consolei de administrare Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555390"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="ecb61-102">Probleme la utilizarea consolei de administrare Intune</span><span class="sxs-lookup"><span data-stu-id="ecb61-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="ecb61-103">**"Acces refuzat" atunci când navigați pe portalul de administrare Intune.**</span><span class="sxs-lookup"><span data-stu-id="ecb61-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="ecb61-104">Dacă sunteți membru al unui rol particularizat Intune, asigurați-vă că contul dvs.</span><span class="sxs-lookup"><span data-stu-id="ecb61-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="ecb61-105">Dacă utilizați Configuration Manager pentru a gestiona dispozitive, verificați dacă nu faceți parte din colecția de utilizatori Intune pentru Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="ecb61-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="ecb61-106">Verificați dacă vi s-au atribuit permisiunile corespunzătoare de control de administrare bazat pe roluri (RBAC) în lama rolurilor Intune.</span><span class="sxs-lookup"><span data-stu-id="ecb61-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="ecb61-107">Verificați dacă grupul utilizat nu este o listă de distribuire.</span><span class="sxs-lookup"><span data-stu-id="ecb61-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="ecb61-108">Intune din portalul Azure acceptă numai conturile de utilizator care aparțin grupurilor de securitate Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ecb61-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="ecb61-109">Examinați grupurile în portalul Azure > **Intune**  >  **Groups**sau în Azure portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="ecb61-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="ecb61-110">**Utilizatorul are prea multe permisiuni pentru rolul Intune atribuit**</span><span class="sxs-lookup"><span data-stu-id="ecb61-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="ecb61-111">Sfătuiți utilizatorul să meargă la **Intune**  >  **Intune roluri**  >  **Permisiunile mele**  >  **Export** pentru a revizui permisiunile acordate.</span><span class="sxs-lookup"><span data-stu-id="ecb61-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="ecb61-112">**Am adăugat un grup de domenii la un rol, dar utilizatorii din acel rol văd în continuare alți utilizatori sau dispozitive.**</span><span class="sxs-lookup"><span data-stu-id="ecb61-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="ecb61-113">Grupurile de domenii nu filtrează utilizatorii sau dispozitivele.</span><span class="sxs-lookup"><span data-stu-id="ecb61-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="ecb61-114">Grupuri de domenii:</span><span class="sxs-lookup"><span data-stu-id="ecb61-114">Scope groups:</span></span>

- <span data-ttu-id="ecb61-115">Limitați utilizatorii cărora le pot atribui politici sau aplicații.</span><span class="sxs-lookup"><span data-stu-id="ecb61-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="ecb61-116">Se permite numai anumitor utilizatori să execute activități la distanță pe dispozitive.</span><span class="sxs-lookup"><span data-stu-id="ecb61-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="ecb61-117">Pentru mai multe informații despre grupurile de domenii, consultați [Controlul accesului bazat pe roluri (RBAC) cu Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ecb61-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ecb61-118">**Am adăugat un utilizator la un rol Intune, dar ei încă mai au acces deplin la consola de admin Intune.**</span><span class="sxs-lookup"><span data-stu-id="ecb61-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="ecb61-119">Navigați la Intune > **Utilizatori în** portalul Azure și verificați dacă utilizatorul nu este asociat la oricare dintre următoarele roluri în portalul Azure:</span><span class="sxs-lookup"><span data-stu-id="ecb61-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="ecb61-120">Administrator global</span><span class="sxs-lookup"><span data-stu-id="ecb61-120">Global administrator</span></span>
- <span data-ttu-id="ecb61-121">Administrator serviciu Intune</span><span class="sxs-lookup"><span data-stu-id="ecb61-121">Intune service administrator</span></span>
- <span data-ttu-id="ecb61-122">Administrator SharePoint</span><span class="sxs-lookup"><span data-stu-id="ecb61-122">SharePoint administrator</span></span>

<span data-ttu-id="ecb61-123">Pentru mai multe informații, consultați [Controlul accesului bazat pe roluri (RBAC) cu Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="ecb61-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ecb61-124">**Probleme de acces**</span><span class="sxs-lookup"><span data-stu-id="ecb61-124">**Access Issues**</span></span>

<span data-ttu-id="ecb61-125">Pentru mai multe informații, consultați [Nu vă puteți conecta la Office 365, Azure sau Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="ecb61-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>