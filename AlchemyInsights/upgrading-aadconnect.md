---
title: 932 actualizarea AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365920"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="8ae0f-102">Upgrade azuriu AD conecta</span><span class="sxs-lookup"><span data-stu-id="8ae0f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="8ae0f-103">În mod implicit, actualizarea automată este activată pentru Azure Connect AD, care ajută pentru a vă asigura că rulaţi cea mai recentă versiune.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="8ae0f-104">Pentru a verifica setările de actualizare automată, utilizaţi cmdletul **Get-ADSyncAutoUpgrade** din PowerShell de AD Azure.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="8ae0f-105">Cmdlet va returna una dintre următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="8ae0f-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="8ae0f-106">**Enabled**: actualizarea automată este activată.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="8ae0f-107">**Cu handicap**: upgrade-ul automat este dezactivat.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="8ae0f-108">**Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="8ae0f-109">Nu pot configura această valoare; Acesta este situat în sistemul de.</span><span class="sxs-lookup"><span data-stu-id="8ae0f-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="8ae0f-110">Pentru informaţii suplimentare, consultaţi [actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="8ae0f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="8ae0f-111">Pentru a descărca cea mai recentă versiune de Azure AD Connect, du-te la [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="8ae0f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
