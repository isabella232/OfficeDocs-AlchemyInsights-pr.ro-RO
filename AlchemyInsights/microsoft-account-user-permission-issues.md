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
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768813"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6715c-102">Depanarea problemei-utilizatorul nu a fost găsit în directorul</span><span class="sxs-lookup"><span data-stu-id="6715c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6715c-103">Dacă utilizatorii primesc mesaj de eroare "utilizatorul nu poate fi găsit" în directorul, vă rugăm să încercați din nou în cazul în care tipul de problemă este utilizator nu în director.</span><span class="sxs-lookup"><span data-stu-id="6715c-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6715c-104">Următorii pași se pot finaliza pentru a depana problema.</span><span class="sxs-lookup"><span data-stu-id="6715c-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6715c-105">Asigurați-vă că contul care a acceptat invitația de e-mail este același cont care este utilizat pentru a face sign in mai târziu.</span><span class="sxs-lookup"><span data-stu-id="6715c-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6715c-106">Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site.</span><span class="sxs-lookup"><span data-stu-id="6715c-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6715c-107">Pentru mai multe informații, consultați [se gestionează aliasuri pentru</a> contul Microsoft pentru a gestiona Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6715c-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6715c-108">Răsfoiți la fiecare site (e) în care utilizatorul primește eroarea.</span><span class="sxs-lookup"><span data-stu-id="6715c-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6715c-109">Adăugați "/_layouts/15/People.aspx/MembershipGroupId = 0" (în ghilimele duble) până la sfârșitul URL-ul site-ului.</span><span class="sxs-lookup"><span data-stu-id="6715c-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6715c-110">Exemplu: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6715c-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6715c-111">Selectați utilizatorul din listă.</span><span class="sxs-lookup"><span data-stu-id="6715c-111">Select the user from the list.</span></span>

- <span data-ttu-id="6715c-112">Faceți clic pe **Eliminare permisiuni utilizator** din panglică.</span><span class="sxs-lookup"><span data-stu-id="6715c-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6715c-113">Adăugați înapoi utilizatorul și Retrimi invitația la utilizator.</span><span class="sxs-lookup"><span data-stu-id="6715c-113">Add back the User and Resend the invite to the user.</span></span>

