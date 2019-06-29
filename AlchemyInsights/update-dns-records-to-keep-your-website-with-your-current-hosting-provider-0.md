---
title: Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353189"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="526cc-102">Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent</span><span class="sxs-lookup"><span data-stu-id="526cc-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="526cc-103">În pagina [domenii](https://portal.office.com/adminportal/home#/Domains) , în lista de domenii, selectaţi domeniul utilizaţi pentru site-ul dumneavoastră, şi apoi selectaţi **Setări DNS** în panoul de administrare.</span><span class="sxs-lookup"><span data-stu-id="526cc-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="526cc-104">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="526cc-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="526cc-105">Pentru **tip DNS** intra: **(adresa)**</span><span class="sxs-lookup"><span data-stu-id="526cc-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="526cc-106">Pentru **gazdă nume sau Alias**, tastaţi următoarele:**@**</span><span class="sxs-lookup"><span data-stu-id="526cc-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="526cc-107">Pentru **Adresa IP**, tastaţi adresa IP statică pentru site-ul dvs., în cazul în care este în prezent găzduit (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="526cc-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="526cc-108">Acest lucru trebuie să fie o adresă IP *statică* pentru site-ul, nu o adresă IP *dinamică* .</span><span class="sxs-lookup"><span data-stu-id="526cc-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="526cc-109">Consultaþi site-ul unde este gazduit site-ul dvs să vă asiguraţi că puteţi obţine o adresă IP statică pentru site-ul dumneavoastră publice.</span><span class="sxs-lookup"><span data-stu-id="526cc-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="526cc-110">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="526cc-110">Select **Save**.</span></span>

<span data-ttu-id="526cc-111">În plus, creaţi o înregistrare CNAME pentru a ajuta clienţii găsi site-ul dvs.</span><span class="sxs-lookup"><span data-stu-id="526cc-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="526cc-112">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="526cc-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="526cc-113">Pentru **tip DNS** intra: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="526cc-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="526cc-114">Pentru **gazdă nume sau Alias**, tastaţi următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="526cc-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="526cc-115">Pentru **puncte la adresă**, tastaţi numele de domeniu complet (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="526cc-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="526cc-116">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="526cc-116">Select **Save**.</span></span>
