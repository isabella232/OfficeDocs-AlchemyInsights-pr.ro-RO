---
title: Ștergerea entității găzduite
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564883"
---
# <a name="delete-tenant"></a><span data-ttu-id="544cc-102">Ștergerea entității găzduite</span><span class="sxs-lookup"><span data-stu-id="544cc-102">Delete tenant</span></span>

<span data-ttu-id="544cc-103">Pentru a șterge o reclamă Azure, asigurați-vă:</span><span class="sxs-lookup"><span data-stu-id="544cc-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="544cc-104">Sunteți administrator global în director.</span><span class="sxs-lookup"><span data-stu-id="544cc-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="544cc-105">Nu sunteți conectat cu un cont care are directorul implicit, cum ar fi contoso.onmicrosoft.com, în contul conectat, cum ar fi admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="544cc-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="544cc-106">Eliminați toate aplicațiile active din Director înainte de ștergere.</span><span class="sxs-lookup"><span data-stu-id="544cc-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="544cc-107">Pentru a elimina aplicațiile active, navigați la înregistrările aplicațiilor și eliminați aplicațiile existente.</span><span class="sxs-lookup"><span data-stu-id="544cc-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="544cc-108">Nu există abonamente active pentru toate serviciile online Microsoft, cum ar fi Microsoft Azure, Office 365 sau Azure AD Premium asociate în director.</span><span class="sxs-lookup"><span data-stu-id="544cc-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="544cc-109">Transferați abonamentele sau grăbiți anularea abonamentelor active prin suportul Azure și facturare.</span><span class="sxs-lookup"><span data-stu-id="544cc-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="544cc-110">Aflați mai multe despre cum să anulați abonamentele Office 365 și Azure.</span><span class="sxs-lookup"><span data-stu-id="544cc-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="544cc-111">Pentru instrucțiuni despre asocierea sau adăugarea unui abonament existent la o entitate găzduită, consultați [asocierea sau adăugarea unui abonament Azure la entitatea găzduită AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="544cc-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="544cc-112">Nu există nicio licență activă.</span><span class="sxs-lookup"><span data-stu-id="544cc-112">There are no Active license.</span></span> <span data-ttu-id="544cc-113">Pentru a elimina licențele, consultați [cum să eliminați abonamentul pentru a elimina licența](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="544cc-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="544cc-114">Nu există alți utilizatori activi în director, în afară de dvs., ca administrator global atunci când încercați să ștergeți reclama Azure.</span><span class="sxs-lookup"><span data-stu-id="544cc-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="544cc-115">Eliminați orice alți utilizatori activi și toate dependențele unui nume de domeniu particularizat din entitatea găzduită vor trebui, de asemenea, eliminate, cum ar fi utilizatorii creați cu admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="544cc-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="544cc-116">Pentru mai multe detalii despre cum să procedați:</span><span class="sxs-lookup"><span data-stu-id="544cc-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="544cc-117">Ștergeți "Azure Active Directory" sau "abonament", consultați [ștergerea Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="544cc-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="544cc-118">Eliminarea aplicațiilor din Director, consultați [eliminarea aplicațiilor](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="544cc-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
