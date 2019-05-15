---
title: Site-ul modernă ca site-ul rădăcină
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057759"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="fc200-102">Site-ul modernă ca site-ul rădăcină</span><span class="sxs-lookup"><span data-stu-id="fc200-102">Modern site as root site</span></span>

<span data-ttu-id="fc200-103">[Lansare ţintă](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) clienţii pot permite acum experienţă de site-ul moderne de comunicare la site-ul clasic rădăcină lor chiriaş de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fc200-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="fc200-104">Această caracteristică poate fi activată prin rularea un cmdlet PowerShell simplu.</span><span class="sxs-lookup"><span data-stu-id="fc200-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="fc200-105">La executarea cu succes a PowerShell command(s), site-ul rădăcină va avea o nouă comunicare-site-ul initiala.</span><span class="sxs-lookup"><span data-stu-id="fc200-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="fc200-106">Detalii despre cerinţele PowerShell cmdlet şi caracteristică sunt disponibile în articol [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="fc200-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="fc200-107">Ne va fi treptat rulare acest lucru, off implicit, orientate versiune clienţilor în 2019 mai devreme, şi rola vor fi disponibile în întreaga lume, până la sfârşitul lunii iunie 2019.</span><span class="sxs-lookup"><span data-stu-id="fc200-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="fc200-108">Continua să se refere la [Centru de mesaje](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) pentru alte caracteristici noi cu cel Modern.</span><span class="sxs-lookup"><span data-stu-id="fc200-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="fc200-109">**Important**: nu ştergeţi site-ul clasic rădăcină pentru a crea un Site de comunicare moderne.</span><span class="sxs-lookup"><span data-stu-id="fc200-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="fc200-110">Acest lucru nu este acceptată de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fc200-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="fc200-111">Ştergerea site-ul rădăcină va face toate site-urile SharePoint din organizaţie inaccesibile pentru toţi utilizatorii, până la restaurarea site-ul sau de a crea un site nou la aceeaşi adresă URL.</span><span class="sxs-lookup"><span data-stu-id="fc200-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 