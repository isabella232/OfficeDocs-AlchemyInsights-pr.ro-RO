---
title: Cod de eroare 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388257"
---
<span data-ttu-id="7423a-103">Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.</span><span class="sxs-lookup"><span data-stu-id="7423a-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="7423a-104">**Registru cheie**</span><span class="sxs-lookup"><span data-stu-id="7423a-104">**Registry key**</span></span>|<span data-ttu-id="7423a-105">**Tip**</span><span class="sxs-lookup"><span data-stu-id="7423a-105">**Type**</span></span>|<span data-ttu-id="7423a-106">**Valoarea**</span><span class="sxs-lookup"><span data-stu-id="7423a-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7423a-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="7423a-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="7423a-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7423a-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="7423a-109">1</span><span class="sxs-lookup"><span data-stu-id="7423a-109">1</span></span>  <br/> |

<span data-ttu-id="7423a-110">Pentru informaţii suplimentare, consultaţi [Permite autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="7423a-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="7423a-111">Monica este activată în mod implicit în Office 365 ProPlus şi Office 2016.</span><span class="sxs-lookup"><span data-stu-id="7423a-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="7423a-112">> remote Desktop servicii (RDS) a fost numit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="7423a-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  