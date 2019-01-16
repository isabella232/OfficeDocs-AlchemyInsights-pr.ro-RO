---
title: Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307012"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="d17ff-102">Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent</span><span class="sxs-lookup"><span data-stu-id="d17ff-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="d17ff-103">În pagina [domenii](https://portal.office.com/adminportal/home#/Domains) , în lista de domenii, selectaţi domeniul utilizaţi pentru site-ul dumneavoastră, şi apoi selectaţi **Setări DNS** în panoul de administrare.</span><span class="sxs-lookup"><span data-stu-id="d17ff-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="d17ff-104">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="d17ff-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="d17ff-105">Pentru **tip DNS** intra: **(adresa)**</span><span class="sxs-lookup"><span data-stu-id="d17ff-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="d17ff-106">Pentru **gazdă nume sau Alias**, tastaţi următoarele:**@**</span><span class="sxs-lookup"><span data-stu-id="d17ff-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="d17ff-107">Pentru **Adresa IP**, tastaţi adresa IP statică pentru site-ul dvs., în cazul în care este în prezent găzduit (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="d17ff-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="d17ff-p101">Acest lucru trebuie să fie o adresă IP *statică* pentru site-ul, nu o adresă IP *dinamică* . Consultaþi site-ul unde este gazduit site-ul dvs să vă asiguraţi că puteţi obţine o adresă IP statică pentru site-ul dumneavoastră publice.</span><span class="sxs-lookup"><span data-stu-id="d17ff-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="d17ff-110">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="d17ff-110">Select **Save**.</span></span> 
    
<span data-ttu-id="d17ff-111">În plus, creaţi o înregistrare CNAME pentru a ajuta clienţii găsi site-ul dvs.</span><span class="sxs-lookup"><span data-stu-id="d17ff-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="d17ff-112">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="d17ff-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="d17ff-113">Pentru **tip DNS** intra: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="d17ff-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="d17ff-114">Pentru **gazdă nume sau Alias**, tastaţi următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="d17ff-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="d17ff-115">Pentru **puncte la adresă**, tastaţi numele de domeniu complet (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d17ff-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="d17ff-116">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="d17ff-116">Select **Save**.</span></span> 
    

