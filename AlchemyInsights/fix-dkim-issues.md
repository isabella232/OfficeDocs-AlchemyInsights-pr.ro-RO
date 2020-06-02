---
title: Remedierea problemelor de instalare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506786"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="e44b8-102">Remedierea problemelor de instalare DKIM</span><span class="sxs-lookup"><span data-stu-id="e44b8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="e44b8-103">Dacă întâmpinați probleme care permit DKIM pentru domeniul particularizat, utilizați următorii pași:</span><span class="sxs-lookup"><span data-stu-id="e44b8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="e44b8-104">Cele mai multe probleme de instalare DKIM sunt legate de înregistrări DNS incorecte.</span><span class="sxs-lookup"><span data-stu-id="e44b8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="e44b8-105">Verificați înregistrarea DKIM CNAME **(nu** o înregistrare TXT) este formatat corect.</span><span class="sxs-lookup"><span data-stu-id="e44b8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e44b8-106">Pentru mai multe informații, consultați acest [subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="e44b8-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="e44b8-107">După ce creați sau actualizați înregistrările DKIM DNS la serviciul de găzduire DNS pentru domeniul dvs., așteptați ca înregistrările DNS să se propage.</span><span class="sxs-lookup"><span data-stu-id="e44b8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="e44b8-108">Dacă nu se pot crea înregistrările DKIM DNS în centrul de administrare, aveți posibilitatea să \<CustomDomain\> înlocuiți cu domeniul particularizat (de exemplu, contoso.com) și să executați această comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="e44b8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
