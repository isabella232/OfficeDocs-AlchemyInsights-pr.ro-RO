---
title: Doar în citire pentru întreținere mesaj atunci când încercați să utilizați SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051293"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="03cb5-102">Doar în citire pentru întreținere mesaj atunci când încercați să utilizați SharePoint sau OneDrive</span><span class="sxs-lookup"><span data-stu-id="03cb5-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="03cb5-103">Utilizatorii pot primi un mesaj **doar în citire pentru întreținere** atunci când încercați să utilizați SharePoint sau OneDrive pentru unul dintre următoarele scenarii.</span><span class="sxs-lookup"><span data-stu-id="03cb5-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="03cb5-104">O activitate de întreținere planificată sau activă.</span><span class="sxs-lookup"><span data-stu-id="03cb5-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="03cb5-105">Verificați-le navigând la [Centrul de mesaje](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="03cb5-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="03cb5-106">Un incident de serviciu activ, de înaltă prioritate, care poate apărea.</span><span class="sxs-lookup"><span data-stu-id="03cb5-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="03cb5-107">Verificați pentru orice recomandări/incidente prin navigarea la [serviciul de sănătate](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="03cb5-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="03cb5-108">Un minor auto-vindecare scenariu de recuperare care ar putea fi întâmplă din cauza oricăror evenimente neașteptate pe serverele care ar putea dura mai puțin de 30 min sau cam asa ceva.</span><span class="sxs-lookup"><span data-stu-id="03cb5-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="03cb5-109">Nu există mesaje centrul de mesaje sau servicii de sănătate pentru aceste recuperări minore, dar ar trebui să fie înapoi la normal foarte curând.</span><span class="sxs-lookup"><span data-stu-id="03cb5-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="03cb5-110">În foarte puține ocazii am observat că unul dintre cele trei scenarii enumerate mai sus au fost cauza, și serviciul a fost restaurat, dar cache-ul utilizatorilor browser-ul nu a fost clarificat.</span><span class="sxs-lookup"><span data-stu-id="03cb5-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="03cb5-111">Vă rugăm să încercați să goliți memoria cache a browserului înainte de a naviga pe site.</span><span class="sxs-lookup"><span data-stu-id="03cb5-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="03cb5-112">În browserul Microsoft Edge, selectați **Setări**, apoi selectați **confidențialitate și securitate**.</span><span class="sxs-lookup"><span data-stu-id="03cb5-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="03cb5-113">Sub **Navigare clară**, selectați **Alegeți ce să goliți**.</span><span class="sxs-lookup"><span data-stu-id="03cb5-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="03cb5-114">Selectați **cookie-uri și date salvate pe site-ul web**și selectați **Golire**.</span><span class="sxs-lookup"><span data-stu-id="03cb5-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="03cb5-115">Acești pași pot diferi atunci când se utilizează alte browsere, ar fi Mozilla Firefox sau Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="03cb5-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="03cb5-116">O altă opțiune ar fi să deschideți site-ul SharePoint sau OneDrive într-o fereastră InPrivate nouă.</span><span class="sxs-lookup"><span data-stu-id="03cb5-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>