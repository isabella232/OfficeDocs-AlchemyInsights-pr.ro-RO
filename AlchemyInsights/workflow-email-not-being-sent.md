---
title: E-mailul fluxului de lucru nu este trimis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766145"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="2b952-102">E-mailul fluxului de lucru nu este trimis pentru o listă sau o bibliotecă SharePoint</span><span class="sxs-lookup"><span data-stu-id="2b952-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="2b952-103">E-mailul din fluxurile de lucru nu este trimis tuturor utilizatorilor sau numai anumitor utilizatori sau vedeți **eroarea Mesajul de poștă electronică nu poate fi trimis. Asigurați-vă că poșta electronică are un destinatar valid**.</span><span class="sxs-lookup"><span data-stu-id="2b952-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="2b952-104">Verificați dacă utilizatorul există în grupul permisiuni **toate persoanele** (lista de informații de utilizator) pentru colecția de site-uri respectivă.</span><span class="sxs-lookup"><span data-stu-id="2b952-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="2b952-105">Exemplu de URL<tenant>direct: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembruGroupId=0</span><span class="sxs-lookup"><span data-stu-id="2b952-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="2b952-106">Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat la pagină.</span><span class="sxs-lookup"><span data-stu-id="2b952-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="2b952-107">Dacă este un utilizator extern, asigurați-vă că invitația lor a fost acceptată.</span><span class="sxs-lookup"><span data-stu-id="2b952-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="2b952-108">Dacă utilizatorul există în grupul de permisiuni, asigurați-vă că adresa de e-mail este corectă.</span><span class="sxs-lookup"><span data-stu-id="2b952-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="2b952-109">Dacă adresa de e-mail a utilizatorilor nu este setată aici, creați o avertizare eșantion pentru acel utilizator care forțează sincronizarea acelui cont de utilizator din profilurile de utilizator sharepoint la această colecție de site-uri.</span><span class="sxs-lookup"><span data-stu-id="2b952-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="2b952-110">E-mail de la fluxuri le-a trimis administratorilor colecției de site-uri, dar nu și altor utilizatori și a vedea eroarea **HTTP Interzis la <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="2b952-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="2b952-111">Consultați [Acces refuzat atunci când trimiteți un e-mail unui grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="2b952-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="2b952-112">De asemenea, verificați că caracteristica **limitată de blocare permisiuneutilizator modul de blocare** colecție de site-ul nu este activ.</span><span class="sxs-lookup"><span data-stu-id="2b952-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="2b952-113">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="2b952-113">Related topics</span></span>
<span data-ttu-id="2b952-114">Doriți să încercați Microsoft Flow în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2b952-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2b952-115">Creare flux</span><span class="sxs-lookup"><span data-stu-id="2b952-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2b952-116">SharePoint și Flux</span><span class="sxs-lookup"><span data-stu-id="2b952-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


