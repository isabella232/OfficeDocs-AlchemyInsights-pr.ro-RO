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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506419"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="f6f2a-102">Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent</span><span class="sxs-lookup"><span data-stu-id="f6f2a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="f6f2a-103">În pagina [domenii](https://portal.office.com/adminportal/home#/Domains) , în lista de domenii, selectaţi domeniul pe care îl utilizaţi pentru site-ul dvs.</span><span class="sxs-lookup"><span data-stu-id="f6f2a-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="f6f2a-104">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="f6f2a-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f6f2a-105">Pentru **tip DNS** intra: **(adresa)**</span><span class="sxs-lookup"><span data-stu-id="f6f2a-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="f6f2a-106">Pentru **gazdă nume sau Alias**, tastaţi următoarele:**@**</span><span class="sxs-lookup"><span data-stu-id="f6f2a-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="f6f2a-107">Pentru **Adresa IP**, tastaţi adresa IP statică pentru site-ul dvs., în cazul în care este în prezent găzduit (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="f6f2a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="f6f2a-108">Acest lucru trebuie să fie o adresă IP *statică* pentru site-ul, nu o adresă IP *dinamică* .</span><span class="sxs-lookup"><span data-stu-id="f6f2a-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="f6f2a-109">Consultaþi site-ul unde este gazduit site-ul dvs să vă asiguraţi că puteţi obţine o adresă IP statică pentru site-ul dumneavoastră publice.</span><span class="sxs-lookup"><span data-stu-id="f6f2a-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="f6f2a-110">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="f6f2a-110">Select **Save**.</span></span>

<span data-ttu-id="f6f2a-111">În plus, creaţi o înregistrare CNAME pentru a ajuta clienţii găsi site-ul dvs.</span><span class="sxs-lookup"><span data-stu-id="f6f2a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="f6f2a-112">Selectaţi **+ nou record personalizat** şi introduceţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="f6f2a-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f6f2a-113">Pentru **tip DNS** intra: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="f6f2a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="f6f2a-114">Pentru **gazdă nume sau Alias**, tastaţi următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="f6f2a-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="f6f2a-115">Pentru **puncte la adresă**, tastaţi numele de domeniu complet (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f6f2a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="f6f2a-116">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="f6f2a-116">Select **Save**.</span></span>
