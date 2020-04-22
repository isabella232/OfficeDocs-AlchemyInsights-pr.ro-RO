---
title: Depanarea problemei - Utilizatorul nu a fost găsit în director
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702750"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="e3f72-102">Depanarea problemei - Utilizatorul nu a fost găsit în director</span><span class="sxs-lookup"><span data-stu-id="e3f72-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="e3f72-103">Dacă utilizatorii primesc mesajul de eroare "utilizatorul nu poate fi găsit" în director, încercați din nou în cazul în care tipul de problemă este utilizatorul nu în director.</span><span class="sxs-lookup"><span data-stu-id="e3f72-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="e3f72-104">Următorii pași pot fi finalizate pentru a depana problema.</span><span class="sxs-lookup"><span data-stu-id="e3f72-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="e3f72-105">Asigurați-vă că contul care a acceptat invitația de e-mail este același cont care este utilizat pentru a vă conecta mai târziu.</span><span class="sxs-lookup"><span data-stu-id="e3f72-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="e3f72-106">Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site.</span><span class="sxs-lookup"><span data-stu-id="e3f72-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="e3f72-107">Pentru mai multe informații, consultați [Cum se</a> gestionează aliasurile pentru contul Microsoft pentru a gestiona conectarea Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="e3f72-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="e3f72-108">Răsfoiți la fiecare site-uri în care utilizatorul primește eroarea.</span><span class="sxs-lookup"><span data-stu-id="e3f72-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="e3f72-109">Adăugați "/_layouts/15/people.aspx/membershipgroupid=0" (în cadrul ghilimelelor duble) la sfârșitul URL-ului site-ului.</span><span class="sxs-lookup"><span data-stu-id="e3f72-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="e3f72-110">Exemplu: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="e3f72-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="e3f72-111">Selectați utilizatorul din listă.</span><span class="sxs-lookup"><span data-stu-id="e3f72-111">Select the user from the list.</span></span>

- <span data-ttu-id="e3f72-112">Faceți clic pe **Eliminare permisiuni utilizator** din panglică.</span><span class="sxs-lookup"><span data-stu-id="e3f72-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="e3f72-113">Adăugați înapoi utilizatorul și retrimite invitația la utilizator.</span><span class="sxs-lookup"><span data-stu-id="e3f72-113">Add back the User and Resend the invite to the user.</span></span>

