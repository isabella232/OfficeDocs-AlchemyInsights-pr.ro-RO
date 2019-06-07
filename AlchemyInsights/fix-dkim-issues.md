---
title: Repara problemele de configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765329"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="d9cbe-102">Repara problemele de configurare DKIM</span><span class="sxs-lookup"><span data-stu-id="d9cbe-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="d9cbe-103">Dacă vă confruntaţi cu probleme care să permită DKIM pentru domeniu personalizat, utilizaţi paşii următori:</span><span class="sxs-lookup"><span data-stu-id="d9cbe-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="d9cbe-104">Cele mai multe probleme de configurare DKIM sunt legate de înregistrări DNS incorecte.</span><span class="sxs-lookup"><span data-stu-id="d9cbe-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="d9cbe-105">Verificaţi dacă înregistrarea DKIM CNAME (**nu** o înregistrare TXT) este formatat corect.</span><span class="sxs-lookup"><span data-stu-id="d9cbe-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d9cbe-106">Pentru informaţii suplimentare, consultaţi acest [subiect](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d9cbe-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="d9cbe-107">După ce creaţi sau actualizaţi înregistrări DKIM DNS la serviciul pentru domeniu (de obicei, Registratorul de domeniu) de găzduire DNS, aşteptaţi pentru înregistrările DNS pentru a propaga.</span><span class="sxs-lookup"><span data-stu-id="d9cbe-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="d9cbe-108">Dacă nu puteţi crea DKIM DNS records în centrul de admin, aveţi posibilitatea să înlocuiţi \<CustomDomain\> cu domeniu personalizat (de exemplu, contoso.com) şi rulaţi această comandă în [PowerShell Online de schimb](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="d9cbe-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
