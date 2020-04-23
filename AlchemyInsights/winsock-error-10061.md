---
title: 1554 Winsock eroare 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766181"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="551f8-102">Eroare Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="551f8-102">Winsock error 10061</span></span>

<span data-ttu-id="551f8-103">Acest cod de eroare înseamnă că Microsoft nu a putut stabili un socket TCP (conexiune) cu gazda țintă.</span><span class="sxs-lookup"><span data-stu-id="551f8-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="551f8-104">Cauza cea mai probabilă a acestei erori este o problemă cu configurația paravanului de protecție.</span><span class="sxs-lookup"><span data-stu-id="551f8-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="551f8-105">Pentru a remedia problema, verificați aceste setări:</span><span class="sxs-lookup"><span data-stu-id="551f8-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="551f8-106">Verificați configurația paravanului de protecție cu informațiile din [url-urile Microsoft 365 și intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="551f8-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="551f8-107">Dacă eroarea este specifică Exchange Online Protection (EOP), ar fi trebuit să fi fost notificat anterior la o modificare a [adreselor IP Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="551f8-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="551f8-108">Verificați că furnizorul de servicii Internet (ISP) nu blochează portul.</span><span class="sxs-lookup"><span data-stu-id="551f8-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="551f8-109">Verificați setările inteligente de gazdă și server țintă în conectori.</span><span class="sxs-lookup"><span data-stu-id="551f8-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="551f8-110">Rețineți că Microsoft 365 nu blochează *conexiunile primite* în acest mod.</span><span class="sxs-lookup"><span data-stu-id="551f8-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
