---
title: Politicile pentru parole
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747050"
---
# <a name="password-policies"></a><span data-ttu-id="29980-102">Politicile pentru parole</span><span class="sxs-lookup"><span data-stu-id="29980-102">Password policies</span></span>

<span data-ttu-id="29980-103">**Am probleme cu Politica de parolă pentru un utilizator**</span><span class="sxs-lookup"><span data-stu-id="29980-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="29980-104">Politica de parolă pentru un utilizator depinde de faptul dacă utilizatorul este doar în cloud sau local.</span><span class="sxs-lookup"><span data-stu-id="29980-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="29980-105">Numai utilizatorii din cloud trebuie să aleagă o parolă care îndeplinește cerințele din acest articol: [politicile de parole care se aplică doar pentru conturile de utilizator din cloud](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="29980-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="29980-106">Utilizatorii locali trebuie să aleagă o parolă care îndeplinește cerințele locale.</span><span class="sxs-lookup"><span data-stu-id="29980-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="29980-107">Dacă un utilizator local nu reușește să își seteze parola, verificați cerințele locale.</span><span class="sxs-lookup"><span data-stu-id="29980-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="29980-108">**Nu știu cum să setez sau să verific politicile de expirare a parolei**</span><span class="sxs-lookup"><span data-stu-id="29980-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="29980-109">Puteți să setați și să verificați politica de expirare pentru utilizatorii în cloud din entitatea găzduită, utilizând PowerShell.</span><span class="sxs-lookup"><span data-stu-id="29980-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="29980-110">Urmați instrucțiunile din acest articol: [Setarea sau verificarea politicilor de parolă utilizând PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="29980-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="29980-111">Politica de expirare a parolei pentru utilizatorii locali este setată în reclama locală.</span><span class="sxs-lookup"><span data-stu-id="29980-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="29980-112">**Alte Linkuri utile:**</span><span class="sxs-lookup"><span data-stu-id="29980-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="29980-113">Introducere în resetarea parolei</span><span class="sxs-lookup"><span data-stu-id="29980-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="29980-114">Depanarea resetării parolei inițiate de administrator</span><span class="sxs-lookup"><span data-stu-id="29980-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
