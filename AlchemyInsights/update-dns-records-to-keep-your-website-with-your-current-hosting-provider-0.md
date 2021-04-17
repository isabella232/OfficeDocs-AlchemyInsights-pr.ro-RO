---
title: Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827542"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="a84fa-102">Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web</span><span class="sxs-lookup"><span data-stu-id="a84fa-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="a84fa-103">În centrul de administrare Microsoft 365, accesați pagina **Configurare** domenii și, în lista de domenii, selectați domeniul pe care îl utilizați pentru  >  [](https://admin.microsoft.com/Adminportal#/Domains) site-ul dvs. web.</span><span class="sxs-lookup"><span data-stu-id="a84fa-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="a84fa-104">Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="a84fa-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a84fa-105">Pentru **Tip DNS,** introduceți: **A (Adresă)**</span><span class="sxs-lookup"><span data-stu-id="a84fa-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="a84fa-106">Pentru **Nume gazdă sau Alias,** tastați următoarele: **@**</span><span class="sxs-lookup"><span data-stu-id="a84fa-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="a84fa-107">Pentru **Adresă IP**, tastați adresa IP statică pentru site-ul dvs. web unde este găzduit în prezent (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="a84fa-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="a84fa-108">Aceasta trebuie să fie o adresă IP  *statică*  pentru site-ul web, nu o  *adresă*  IP dinamică.</span><span class="sxs-lookup"><span data-stu-id="a84fa-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="a84fa-109">Consultați site-ul în care este găzduit site-ul web, pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.</span><span class="sxs-lookup"><span data-stu-id="a84fa-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="a84fa-110">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="a84fa-110">Select **Save**.</span></span>

<span data-ttu-id="a84fa-111">În plus, puteți crea o înregistrare CNAME pentru a-i ajuta pe clienți să vă găsească site-ul web.</span><span class="sxs-lookup"><span data-stu-id="a84fa-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="a84fa-112">Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="a84fa-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a84fa-113">Pentru **Tip DNS introduceți:** **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="a84fa-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="a84fa-114">Pentru **Nume gazdă sau Alias,** tastați următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="a84fa-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="a84fa-115">Pentru **Adresă indicatială,** tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a84fa-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="a84fa-116">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="a84fa-116">Select **Save**.</span></span>
