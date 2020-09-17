---
title: Actualizarea înregistrărilor DNS pentru a vă menține site-ul web la furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815797"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="6ce04-102">Actualizarea înregistrărilor DNS pentru a vă menține site-ul web la furnizorul de găzduire curent</span><span class="sxs-lookup"><span data-stu-id="6ce04-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="6ce04-103">În centrul de administrare Microsoft 365, accesați **Setup**  >  pagina[Domains](https://admin.microsoft.com/Adminportal#/Domains) setup și, în lista de domenii, selectați domeniul pe care îl utilizați pentru site-ul web.</span><span class="sxs-lookup"><span data-stu-id="6ce04-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="6ce04-104">Selectați **+ înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="6ce04-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="6ce04-105">Pentru **tip DNS** , introduceți: **A (adresă)**</span><span class="sxs-lookup"><span data-stu-id="6ce04-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="6ce04-106">Pentru **nume gazdă sau alias**, tastați următoarele: **@**</span><span class="sxs-lookup"><span data-stu-id="6ce04-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="6ce04-107">Pentru **adresă IP**, tastați adresa IP statică pentru site-ul web unde este găzduit în prezent (de exemplu, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="6ce04-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="6ce04-108">Aceasta trebuie să fie o adresă IP  *statică*  pentru site-ul web, nu o adresă IP  *dinamică*  .</span><span class="sxs-lookup"><span data-stu-id="6ce04-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="6ce04-109">Consultați site-ul unde este găzduit site-ul web pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.</span><span class="sxs-lookup"><span data-stu-id="6ce04-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="6ce04-110">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="6ce04-110">Select **Save**.</span></span>

<span data-ttu-id="6ce04-111">În plus, puteți să creați o înregistrare CNAME pentru a-i ajuta pe clienți să vă găsească site-ul web.</span><span class="sxs-lookup"><span data-stu-id="6ce04-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="6ce04-112">Selectați **+ înregistrare particularizată nouă** și introduceți următoarele:</span><span class="sxs-lookup"><span data-stu-id="6ce04-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="6ce04-113">Pentru **tip DNS** , introduceți: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="6ce04-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="6ce04-114">Pentru **nume gazdă sau alias**, tastați următoarele: **www**</span><span class="sxs-lookup"><span data-stu-id="6ce04-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="6ce04-115">Pentru **adresă de puncte**, tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="6ce04-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="6ce04-116">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="6ce04-116">Select **Save**.</span></span>
