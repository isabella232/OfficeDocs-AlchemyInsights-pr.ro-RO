---
title: 1554 eroare Winsock 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485375"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="35630-102">Eroare Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="35630-102">Winsock error 10061</span></span>

<span data-ttu-id="35630-p101">Acest cod de eroare înseamnă că Office 365 nu a putut stabili un socket TCP (conexiune) cu ţintă gazdă. Cel mai probabil cauza acestei erori este o problemă cu configuraţia paravanului de protecţie. Pentru a remedia problema, verificaţi aceste setări:</span><span class="sxs-lookup"><span data-stu-id="35630-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="35630-106">Verificaţi configuraţia paravanului de protecţie cu informaţii la [Office 365 URL-uri şi intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="35630-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="35630-107">În cazul în care eroarea este specific pentru Exchange Online protecţia (EOP), tu ar trebui să au fost anterior notificate la o schimbare la [adresele IP de protecţie Online Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="35630-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="35630-108">Verificaţi că dumneavoastră Internet Service Provider (ISP) nu este blocarea portului.</span><span class="sxs-lookup"><span data-stu-id="35630-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="35630-109">Verifica smart setările serverului de gazdă şi ţintă, în dumneavoastră conectori.</span><span class="sxs-lookup"><span data-stu-id="35630-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="35630-110">Reţineţi că Biroul 365 nu bloca conexiunile de *intrare* în acest mod.</span><span class="sxs-lookup"><span data-stu-id="35630-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

