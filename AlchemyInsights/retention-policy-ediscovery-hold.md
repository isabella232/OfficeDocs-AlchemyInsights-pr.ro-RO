---
title: 2609-reținere-sau-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994088"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="7d17a-102">Imposibil de șters elemente în SharePoint Online sau OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="7d17a-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="7d17a-103">Tu sau utilizatorii pot fi imposibil să ștergeți elemente în SharePoint Online sau OneDrive for Business, deoarece o politică de retenție, etichetă de conservare sau eDiscovery Hold se aplică la un SharePoint de OneDrive site-ul sau la un anumit element.</span><span class="sxs-lookup"><span data-stu-id="7d17a-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="7d17a-104">Aceasta include imposibilitatea de a șterge un document, o versiune de document, un folder, o bibliotecă de documente, o listă, o aplicație, un site sau o colecție de site-uri.</span><span class="sxs-lookup"><span data-stu-id="7d17a-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="7d17a-105">Iată câteva exemple de mesaje de eroare pe care le-ați primit dacă încercați să ștergeți un element care este reținut:</span><span class="sxs-lookup"><span data-stu-id="7d17a-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="7d17a-106">"Acest site nu poate fi șters, deoarece este inclus într-o politică de așteptare sau retenție eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="7d17a-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="7d17a-107">"Acest site are o politică de conformitate setată la blocarea ștergerii"</span><span class="sxs-lookup"><span data-stu-id="7d17a-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="7d17a-108">"O politică de conformitate blochează în prezent această ștergere de site-ul"</span><span class="sxs-lookup"><span data-stu-id="7d17a-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="7d17a-109">"Această colecție de site-ul nu poate fi șters, deoarece conține site-uri care sunt incluse într-o politică de așteptare sau retenție eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="7d17a-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="7d17a-110">"Trebuie să ștergeți toate elementele din acest folder înainte de a șterge folderul"</span><span class="sxs-lookup"><span data-stu-id="7d17a-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="7d17a-111">"Versiunile de acest element nu pot fi șterse, deoarece este în așteptare sau retenție politica"</span><span class="sxs-lookup"><span data-stu-id="7d17a-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="7d17a-112">"Elementul nu poate fi șters în așteptare"</span><span class="sxs-lookup"><span data-stu-id="7d17a-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="7d17a-113">"Eticheta care se aplică la acest element împiedică editarea sau ștergerea"</span><span class="sxs-lookup"><span data-stu-id="7d17a-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="7d17a-114">"Lista nu poate fi ștearsă în timp ce în așteptare sau Politica de retenție"</span><span class="sxs-lookup"><span data-stu-id="7d17a-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="7d17a-115">"Lista nu poate fi ștearsă dacă este blocată sau dacă se aplică o politică de retenție"</span><span class="sxs-lookup"><span data-stu-id="7d17a-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="7d17a-116">Pentru a șterge elementele dintr-unul dintre aceste scenarii, trebuie eliminată Politica de retenție, eticheta de conservare sau reținerea eDiscovery (sau un site trebuie să fie exclus dintr-o politică de retenție).</span><span class="sxs-lookup"><span data-stu-id="7d17a-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="7d17a-117">Trebuie să dezactivați sau să excludeți respectiva așteptare care cauzează această problemă.</span><span class="sxs-lookup"><span data-stu-id="7d17a-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="7d17a-118">După ce se elimină o politică de retenție sau o așteptare, poate dura până la 24 de ore pentru ca modificarea să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="7d17a-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="7d17a-119">Pentru informații despre diferitele caracteristici de retenție și așteptare care pot fi aplicate la site-uri SharePoint și conturi OneDrive, consultați unul dintre următoarele subiecte.</span><span class="sxs-lookup"><span data-stu-id="7d17a-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="7d17a-120">Prezentare generală a politicilor de conservare</span><span class="sxs-lookup"><span data-stu-id="7d17a-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="7d17a-121">Prezentare generală a etichetelor de retenție</span><span class="sxs-lookup"><span data-stu-id="7d17a-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="7d17a-122">Gestionați deține în Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="7d17a-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="7d17a-123">eDiscovery deține</span><span class="sxs-lookup"><span data-stu-id="7d17a-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="7d17a-124">Politicile de închidere și ștergere a site-ului moștenite</span><span class="sxs-lookup"><span data-stu-id="7d17a-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
