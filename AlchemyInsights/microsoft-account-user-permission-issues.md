---
title: Depanarea problemei-utilizatorul nu a fost găsit în directorul
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754204"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="82ca9-102">Depanarea problemei-utilizatorul nu a fost găsit în directorul</span><span class="sxs-lookup"><span data-stu-id="82ca9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="82ca9-103">Dacă utilizatorii primesc mesaj de eroare "utilizatorul nu poate fi găsit" în directorul.</span><span class="sxs-lookup"><span data-stu-id="82ca9-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="82ca9-104">Încercați din nou în cazul în care tipul de problemă este utilizator nu în director.</span><span class="sxs-lookup"><span data-stu-id="82ca9-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="82ca9-105">Următorii pași se pot finaliza pentru a depana problema.</span><span class="sxs-lookup"><span data-stu-id="82ca9-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="82ca9-106">Asigurați-vă că contul care a acceptat invitația de e-mail este același cont care este utilizat pentru a face sign in mai târziu.</span><span class="sxs-lookup"><span data-stu-id="82ca9-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="82ca9-107">Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site.</span><span class="sxs-lookup"><span data-stu-id="82ca9-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="82ca9-108">Pentru mai multe informații, consultați [se gestionează aliasuri pentru</a> contul Microsoft pentru a gestiona Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="82ca9-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="82ca9-109">Răsfoiți la fiecare site (e) în care utilizatorul primește eroarea.</span><span class="sxs-lookup"><span data-stu-id="82ca9-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="82ca9-110">Adăugați "/_layout/15/People.aspx/MembershipGroupId = 0" (în ghilimele duble) până la sfârșitul adresei URL a site-ului.</span><span class="sxs-lookup"><span data-stu-id="82ca9-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="82ca9-111">Exemplu: https://_ _ \ "Contosoa _ Gt_. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="82ca9-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="82ca9-112">Selectați utilizatorul din listă.</span><span class="sxs-lookup"><span data-stu-id="82ca9-112">Select the user from the list.</span></span>

- <span data-ttu-id="82ca9-113">Faceți clic pe **Eliminare permisiuni utilizator** din panglică.</span><span class="sxs-lookup"><span data-stu-id="82ca9-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="82ca9-114">Adăugați înapoi utilizatorul și Retrimi invitația la utilizator.</span><span class="sxs-lookup"><span data-stu-id="82ca9-114">Add back the User and Resend the invite to the user.</span></span>

