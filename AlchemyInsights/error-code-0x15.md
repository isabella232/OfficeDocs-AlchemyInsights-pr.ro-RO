---
title: Cod de eroare 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402751"
---
<span data-ttu-id="15941-103">Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.</span><span class="sxs-lookup"><span data-stu-id="15941-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="15941-104">**Registru cheie**</span><span class="sxs-lookup"><span data-stu-id="15941-104">**Registry key**</span></span>|<span data-ttu-id="15941-105">**Tip**</span><span class="sxs-lookup"><span data-stu-id="15941-105">**Type**</span></span>|<span data-ttu-id="15941-106">**Valoarea**</span><span class="sxs-lookup"><span data-stu-id="15941-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="15941-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="15941-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="15941-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="15941-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="15941-109">1</span><span class="sxs-lookup"><span data-stu-id="15941-109">1</span></span>  <br/> |
   
<span data-ttu-id="15941-110">Pentru informaţii suplimentare, consultaţi [Permite autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="15941-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="15941-111">Monica este activată în mod implicit în Office 365 ProPlus şi Office 2016.</span><span class="sxs-lookup"><span data-stu-id="15941-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="15941-112">> remote Desktop servicii (RDS) a fost numit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="15941-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

