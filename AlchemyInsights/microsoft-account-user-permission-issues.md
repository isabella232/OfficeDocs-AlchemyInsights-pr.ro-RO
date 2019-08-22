---
title: Depanaţi problema - utilizatorul nu a fost găsit în Director
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544875"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="25e3d-102">Depanaţi problema - utilizatorul nu a fost găsit în Director</span><span class="sxs-lookup"><span data-stu-id="25e3d-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="25e3d-103">În cazul în care utilizatorii primesc eroare mesajul "utilizator nu poate fi găsit" în directorul.</span><span class="sxs-lookup"><span data-stu-id="25e3d-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="25e3d-104">Vă rugăm să încercaţi din nou în cazul în care problema de tip utilizator nu este în director.</span><span class="sxs-lookup"><span data-stu-id="25e3d-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="25e3d-105">Paşii de mai jos poate fi terminat pentru a depana problema.</span><span class="sxs-lookup"><span data-stu-id="25e3d-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="25e3d-106">Asigura contului care a acceptat invitaţia e-mail este acelaşi cont, care este folosit să semneze mai târziu.</span><span class="sxs-lookup"><span data-stu-id="25e3d-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="25e3d-107">Asiguraţi-vă că utilizatorul este folosind acelaşi cont pentru a accepta invita şi conectaţi-vă site-ul.</span><span class="sxs-lookup"><span data-stu-id="25e3d-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="25e3d-108">Pentru mai multe informaţii, consultaţi [Cum de a gestiona pseudonime pentru contul dumneavoastră Microsoft</a> pentru a gestiona logare Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="25e3d-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="25e3d-109">Navigaţi la fiecare site în care utilizatorul primeşte eroare.</span><span class="sxs-lookup"><span data-stu-id="25e3d-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="25e3d-110">Adauga "/ _layouts/15/people.aspx/membershipgroupid=0" (la dublu-ghilimele) la sfârşitul URL-ul site-ului.</span><span class="sxs-lookup"><span data-stu-id="25e3d-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="25e3d-111">Exemplu: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="25e3d-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="25e3d-112">Selectaţi utilizator din listă.</span><span class="sxs-lookup"><span data-stu-id="25e3d-112">Select the user from the list.</span></span>

- <span data-ttu-id="25e3d-113">Faceţi clic pe **Eliminare permisiuni utilizator** din panglică.</span><span class="sxs-lookup"><span data-stu-id="25e3d-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="25e3d-114">Adauga înapoi utilizatorului şi retrimiteţi a invita pentru utilizator.</span><span class="sxs-lookup"><span data-stu-id="25e3d-114">Add back the User and Resend the invite to the user.</span></span>

