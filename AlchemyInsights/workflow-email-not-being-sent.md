---
title: E-mailul fluxului de lucru nu este trimis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049385"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a3c42-102">E-mail de flux de lucru nu este trimis pentru o listă SharePoint sau bibliotecă</span><span class="sxs-lookup"><span data-stu-id="a3c42-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a3c42-103">E-mailurile din fluxuri de lucru nu sunt trimise tuturor utilizatorilor sau numai utilizatorilor specifici sau vedeți eroarea **mesajul de poștă electronică nu poate fi trimis. Asigurați-vă că poșta electronică are un destinatar valid**.</span><span class="sxs-lookup"><span data-stu-id="a3c42-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a3c42-104">Verificați dacă utilizatorul există în grupul de permisiuni **toate persoanele** (lista de informații de utilizator) pentru acea colecție de site-uri.</span><span class="sxs-lookup"><span data-stu-id="a3c42-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a3c42-105">Exemplu de URL direct:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="a3c42-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a3c42-106">Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat în pagină.</span><span class="sxs-lookup"><span data-stu-id="a3c42-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a3c42-107">Dacă este un utilizator extern, asigurați-vă că invitația lor a fost acceptată.</span><span class="sxs-lookup"><span data-stu-id="a3c42-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a3c42-108">Dacă utilizatorul există în grupul de permisiuni, asigurați-vă că adresa de e-mail este corectă.</span><span class="sxs-lookup"><span data-stu-id="a3c42-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a3c42-109">Dacă adresa de e-mail a utilizatorilor nu este setată aici, apoi creați o alertă de eșantion pentru acel utilizator care obligă sincronizarea acelui cont de utilizator din profilurile de utilizator ale SharePoint la această colecție de site-uri.</span><span class="sxs-lookup"><span data-stu-id="a3c42-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a3c42-110">E-mailul din fluxurile de lucru sunt trimise administratorilor de colecție de site-uri, dar nu și altor utilizatori și vedeți eroarea **http interzisă la <span>https:</span>//_vti_bin/client.XVC.SP.Utilities.Utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="a3c42-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a3c42-111">Consultați [acces refuzat atunci când trimiteți un e-mail la un grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a3c42-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a3c42-112">De asemenea, Verificați că caracteristica de colectare a site-ului de **blocare permisiuni de acces limitat de utilizator** nu este activă.</span><span class="sxs-lookup"><span data-stu-id="a3c42-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a3c42-113">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="a3c42-113">Related topics</span></span>
<span data-ttu-id="a3c42-114">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a3c42-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a3c42-115">Creare flux</span><span class="sxs-lookup"><span data-stu-id="a3c42-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a3c42-116">SharePoint și flux</span><span class="sxs-lookup"><span data-stu-id="a3c42-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


