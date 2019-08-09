---
title: Flux de lucru e-mail nu este trimis
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270684"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="ae245-102">Flux de lucru e-mail nu este trimis</span><span class="sxs-lookup"><span data-stu-id="ae245-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="ae245-103">E-mail de la fluxurile de lucru nu sunt trimise tuturor utilizatorilor sau doar anumiţi utilizatori, sau tu a vedea eroare **mesajul de poștă electronică nu poate fi trimis. Asiguraţi-vă că adresa de e-mail a destinatarului valid**.</span><span class="sxs-lookup"><span data-stu-id="ae245-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="ae245-104">Verificaţi dacă utilizatorul există în **Toţi oamenii** permisiunile grupului (lista informații utilizator) pentru că colecției de site-uri.</span><span class="sxs-lookup"><span data-stu-id="ae245-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ae245-105">Proba directă URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ae245-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="ae245-106">În cazul în care utilizatorul nu exista, asiguraţi-vă că utilizatorul este semnat în pagină.</span><span class="sxs-lookup"><span data-stu-id="ae245-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="ae245-107">În cazul în care este un utilizator extern, asiguraţi-vă că invitaţia a fost acceptată.</span><span class="sxs-lookup"><span data-stu-id="ae245-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="ae245-108">Dacă utilizatorul există în grupul de permisiuni, asiguraţi-vă că adresa de e-mail este corectă.</span><span class="sxs-lookup"><span data-stu-id="ae245-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="ae245-109">În cazul în care adresa de e-mail a utilizatorilor nu este stabilit aici, apoi creaţi o alertă de probă pentru acel utilizator care forţele sincronizare acel cont de utilizator la User profile de SharePoint pentru această colecție de site-ul.</span><span class="sxs-lookup"><span data-stu-id="ae245-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ae245-110">E-mail de la fluxuri de lucru sunt trimise la administratori ai colecției de site-ul dar nu de la alţi utilizatori şi vedea de eroare \*\*HTTP interzis să <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="ae245-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="ae245-111">A se vedea [Acces refuzat atunci când grupuri de poştă electronică să](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="ae245-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="ae245-112">De asemenea, să verifice dacă caracteristica de colectare **modul acces limitat utilizator permisiunea lockdown** site-ul nu este activ.</span><span class="sxs-lookup"><span data-stu-id="ae245-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="ae245-113">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="ae245-113">Related topics</span></span>
<span data-ttu-id="ae245-114">Doriţi să încercaţi Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ae245-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ae245-115">Crea fluxul</span><span class="sxs-lookup"><span data-stu-id="ae245-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ae245-116">SharePoint şi fluxul</span><span class="sxs-lookup"><span data-stu-id="ae245-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


