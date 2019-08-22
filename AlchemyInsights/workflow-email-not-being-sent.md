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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530898"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="6031e-102">Flux de lucru e-mail nu este trimis pentru o listă SharePoint sau biblioteca</span><span class="sxs-lookup"><span data-stu-id="6031e-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="6031e-103">E-mail de la fluxurile de lucru nu sunt trimise tuturor utilizatorilor sau doar anumiţi utilizatori, sau tu a vedea eroare **mesajul de poștă electronică nu poate fi trimis. Asiguraţi-vă că adresa de e-mail a destinatarului valid**.</span><span class="sxs-lookup"><span data-stu-id="6031e-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="6031e-104">Verificaţi dacă utilizatorul există în **Toţi oamenii** permisiunile grupului (lista informații utilizator) pentru că colecției de site-uri.</span><span class="sxs-lookup"><span data-stu-id="6031e-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="6031e-105">Proba directă URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="6031e-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="6031e-106">În cazul în care utilizatorul nu exista, asiguraţi-vă că utilizatorul este semnat în pagină.</span><span class="sxs-lookup"><span data-stu-id="6031e-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="6031e-107">În cazul în care este un utilizator extern, asiguraţi-vă că invitaţia a fost acceptată.</span><span class="sxs-lookup"><span data-stu-id="6031e-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="6031e-108">Dacă utilizatorul există în grupul de permisiuni, asiguraţi-vă că adresa de e-mail este corectă.</span><span class="sxs-lookup"><span data-stu-id="6031e-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="6031e-109">În cazul în care adresa de e-mail a utilizatorilor nu este stabilit aici, apoi creaţi o alertă de probă pentru acel utilizator care forţele sincronizare acel cont de utilizator la User profile de SharePoint pentru această colecție de site-ul.</span><span class="sxs-lookup"><span data-stu-id="6031e-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="6031e-110">E-mail de la fluxuri de lucru sunt trimise la administratori ai colecției de site-ul dar nu de la alţi utilizatori şi vedea de eroare **HTTP interzis la <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="6031e-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="6031e-111">A se vedea [Acces refuzat atunci când trimiteţi un mesaj către un grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="6031e-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="6031e-112">De asemenea, să verifice dacă caracteristica de colectare **modul acces limitat utilizator permisiunea lockdown** site-ul nu este activ.</span><span class="sxs-lookup"><span data-stu-id="6031e-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="6031e-113">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="6031e-113">Related topics</span></span>
<span data-ttu-id="6031e-114">Doriţi să încercaţi Flow Microsoft SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6031e-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6031e-115">Crea fluxul</span><span class="sxs-lookup"><span data-stu-id="6031e-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6031e-116">SharePoint şi fluxul</span><span class="sxs-lookup"><span data-stu-id="6031e-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


