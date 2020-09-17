---
title: 932 upgrade-ul AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806051"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f2602-102">Upgrade-ul Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f2602-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f2602-103">În mod implicit, upgrade-ul automat este activat pentru Azure AD Connect, care vă ajută să vă asigurați că rulează cea mai recentă versiune.</span><span class="sxs-lookup"><span data-stu-id="f2602-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f2602-104">Pentru a verifica setările de upgrade automat, utilizați cmdletul **Get-ADSyncAutoUpgrade** din Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f2602-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f2602-105">Cmdletul va returna una dintre următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="f2602-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f2602-106">**Activat**: upgrade-ul automat este activat.</span><span class="sxs-lookup"><span data-stu-id="f2602-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f2602-107">**Dezactivat**: upgrade-ul automat este dezactivat.</span><span class="sxs-lookup"><span data-stu-id="f2602-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f2602-108">**Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate.</span><span class="sxs-lookup"><span data-stu-id="f2602-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f2602-109">Nu puteți configura această valoare; este setat de sistem.</span><span class="sxs-lookup"><span data-stu-id="f2602-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f2602-110">Pentru mai multe informații, consultați upgrade-ul [automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="f2602-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f2602-111">Pentru a descărca cea mai recentă versiune de Azure AD Connect, accesați [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="f2602-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
