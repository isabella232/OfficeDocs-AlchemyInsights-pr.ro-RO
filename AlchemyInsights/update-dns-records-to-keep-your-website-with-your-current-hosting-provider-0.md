---
title: Actualizați înregistrările DNS pentru a vă păstra site-ul web cu furnizorul curent de găzduire
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665772"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="74679-102">Actualizați înregistrările DNS pentru a vă păstra site-ul web cu furnizorul curent de găzduire</span><span class="sxs-lookup"><span data-stu-id="74679-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="74679-103">În centrul de administrare Microsoft 365, accesați pagina Domenii de **instalare**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) și, în lista de domenii, selectați domeniul pe care îl utilizați pentru site-ul dvs.</span><span class="sxs-lookup"><span data-stu-id="74679-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="74679-104">Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="74679-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="74679-105">Pentru **tipul DNS** introduceți: **A (Adresă)**</span><span class="sxs-lookup"><span data-stu-id="74679-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="74679-106">Pentru **nume gazdă sau alias**, tastați următoarele:**@**</span><span class="sxs-lookup"><span data-stu-id="74679-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="74679-107">Pentru **adresa IP**, tastați adresa IP statică pentru site-ul web unde este găzduită în prezent (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="74679-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="74679-108">Aceasta trebuie să fie o adresă IP *statică* pentru site-ul web, nu o adresă IP *dinamică.*</span><span class="sxs-lookup"><span data-stu-id="74679-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="74679-109">Consultați site-ul unde este găzduit site-ul dvs., pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.</span><span class="sxs-lookup"><span data-stu-id="74679-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="74679-110">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="74679-110">Select **Save**.</span></span>

<span data-ttu-id="74679-111">În plus, puteți crea o înregistrare CNAME pentru a ajuta clienții să vă găsească site-ul web.</span><span class="sxs-lookup"><span data-stu-id="74679-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="74679-112">Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="74679-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="74679-113">Pentru **tipul DNS** introduceți: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="74679-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="74679-114">Pentru **nume gazdă sau alias**, tastați următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="74679-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="74679-115">Pentru **puncte de adresă,** tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="74679-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="74679-116">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="74679-116">Select **Save**.</span></span>
