---
title: Remedierea problemelor de configurare DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744962"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="3f3d9-102">Remedierea problemelor de configurare DKIM</span><span class="sxs-lookup"><span data-stu-id="3f3d9-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="3f3d9-103">Dacă întâmpinați probleme care permit DKIM pentru domeniul particularizat, utilizați următorii pași:</span><span class="sxs-lookup"><span data-stu-id="3f3d9-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="3f3d9-104">Majoritatea problemelor de configurare DKIM sunt asociate înregistrărilor DNS incorecte.</span><span class="sxs-lookup"><span data-stu-id="3f3d9-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="3f3d9-105">Verificați dacă înregistrarea CNAME DKIM (**nu** este o înregistrare txt) este formatat corect.</span><span class="sxs-lookup"><span data-stu-id="3f3d9-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="3f3d9-106">Pentru mai multe informații, consultați acest [subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="3f3d9-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="3f3d9-107">După ce creați sau actualizați înregistrările DNS DKIM la serviciul de găzduire DNS pentru domeniul dvs. (de obicei, Registratorul de domeniu), așteptați ca înregistrările DNS să se propage.</span><span class="sxs-lookup"><span data-stu-id="3f3d9-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="3f3d9-108">Dacă nu puteți crea înregistrările DNS DKIM în centrul de administrare, puteți să înlocuiți \<CustomDomain\> cu domeniul particularizat (de exemplu, contoso.com) și să difuzați această comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="3f3d9-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
