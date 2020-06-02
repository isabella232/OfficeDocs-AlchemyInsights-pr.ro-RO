---
title: Cod eroare 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Dacă primiți o eroare la activarea Office 2013 pe implementări de servicii Desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506858"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="931f6-103">Eroare în timpul activării Office 2013 pe servicii Desktop la distanță</span><span class="sxs-lookup"><span data-stu-id="931f6-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="931f6-104">Dacă primiți o eroare la activarea Office 2013 pe implementări de servicii Desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.</span><span class="sxs-lookup"><span data-stu-id="931f6-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="931f6-105">**Cheie de registry**</span><span class="sxs-lookup"><span data-stu-id="931f6-105">**Registry key**</span></span>|<span data-ttu-id="931f6-106">**Tip**</span><span class="sxs-lookup"><span data-stu-id="931f6-106">**Type**</span></span>|<span data-ttu-id="931f6-107">**Valoarea**</span><span class="sxs-lookup"><span data-stu-id="931f6-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="931f6-108">HKEY_CURRENT_USER Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="931f6-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="931f6-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="931f6-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="931f6-110">1</span><span class="sxs-lookup"><span data-stu-id="931f6-110">1</span></span>  <br/> |

<span data-ttu-id="931f6-111">Pentru mai multe informații, consultați [Activarea autentificării moderne pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="931f6-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="931f6-112">ADAL este activat în mod implicit în Microsoft 365 Apps pentru întreprinderi și Office 2016.</span><span class="sxs-lookup"><span data-stu-id="931f6-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="931f6-113">Servicii Desktop la distanță (RDS) a fost denumit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="931f6-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  