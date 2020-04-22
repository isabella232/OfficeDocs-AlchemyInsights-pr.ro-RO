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
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703150"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="a9e53-103">Eroare în timpul activării Office 2013 pe servicii Desktop la distanță</span><span class="sxs-lookup"><span data-stu-id="a9e53-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="a9e53-104">Dacă primiți o eroare la activarea Office 2013 pe implementări de servicii Desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.</span><span class="sxs-lookup"><span data-stu-id="a9e53-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="a9e53-105">**Cheie de registry**</span><span class="sxs-lookup"><span data-stu-id="a9e53-105">**Registry key**</span></span>|<span data-ttu-id="a9e53-106">**Tip**</span><span class="sxs-lookup"><span data-stu-id="a9e53-106">**Type**</span></span>|<span data-ttu-id="a9e53-107">**Valoarea**</span><span class="sxs-lookup"><span data-stu-id="a9e53-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a9e53-108">HKEY_CURRENT_USER Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="a9e53-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="a9e53-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="a9e53-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="a9e53-110">1</span><span class="sxs-lookup"><span data-stu-id="a9e53-110">1</span></span>  <br/> |

<span data-ttu-id="a9e53-111">Pentru mai multe informații, consultați [Activarea autentificării moderne pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a9e53-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="a9e53-112">ADAL este activat în mod implicit în Microsoft 365 Apps pentru întreprinderi și Office 2016.</span><span class="sxs-lookup"><span data-stu-id="a9e53-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="a9e53-113">Servicii Desktop la distanță (RDS) a fost denumit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="a9e53-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  