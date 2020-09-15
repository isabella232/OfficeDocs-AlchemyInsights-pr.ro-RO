---
title: Doar în citire pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670844"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="e55eb-102">Doar în citire pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="e55eb-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="e55eb-103">Utilizatorii pot primi un mesaj **doar în citire pentru întreținere** atunci când încearcă să utilizeze SharePoint sau OneDrive pentru unul dintre următoarele scenarii.</span><span class="sxs-lookup"><span data-stu-id="e55eb-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="e55eb-104">O activitate de întreținere planificată sau activă.</span><span class="sxs-lookup"><span data-stu-id="e55eb-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="e55eb-105">Verificați dacă navigați la [Centrul de mesaje](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="e55eb-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="e55eb-106">Un incident de serviciu activ, prioritar, care poate apărea.</span><span class="sxs-lookup"><span data-stu-id="e55eb-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="e55eb-107">Căutați recomandări/incidente navigând la [starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e55eb-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="e55eb-108">Un scenariu minor de recuperare automată care s-ar putea întâmpla din cauza oricăror evenimente neașteptate de pe serverele care pot dura mai puțin de 30 de minute.</span><span class="sxs-lookup"><span data-stu-id="e55eb-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="e55eb-109">Nu există niciun centru de mesaje sau posturi de stare a serviciului pentru aceste recuperări minore, dar ar trebui să reveniți la normal foarte curând.</span><span class="sxs-lookup"><span data-stu-id="e55eb-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="e55eb-110">În foarte puține ocazii am observat că una dintre cele trei scenarii listate mai sus a fost cauza, iar serviciul a fost restaurat, dar memoria cache a browserului utilizatori nu a fost eliminată.</span><span class="sxs-lookup"><span data-stu-id="e55eb-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="e55eb-111">Încercați să debifați memoria cache a browserului înainte de a naviga la site.</span><span class="sxs-lookup"><span data-stu-id="e55eb-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="e55eb-112">În browserul Microsoft Edge, selectați **Setări**, apoi selectați **confidențialitate și securitate**.</span><span class="sxs-lookup"><span data-stu-id="e55eb-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="e55eb-113">Sub **Ștergere navigare**, selectați **Alegeți ce să goliți**.</span><span class="sxs-lookup"><span data-stu-id="e55eb-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="e55eb-114">Selectați **modulele cookie și datele salvate ale site-urilor web**și selectați **Ștergere**.</span><span class="sxs-lookup"><span data-stu-id="e55eb-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="e55eb-115">Acești pași pot diferi atunci când utilizați alte browsere, cum ar fi Mozilla Firefox sau Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="e55eb-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="e55eb-116">O altă opțiune ar fi să deschideți site-ul SharePoint sau OneDrive într-o fereastră inprivată nouă.</span><span class="sxs-lookup"><span data-stu-id="e55eb-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>