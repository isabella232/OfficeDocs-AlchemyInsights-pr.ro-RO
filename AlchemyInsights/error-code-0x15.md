---
title: Cod de eroare 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307157"
---
<span data-ttu-id="b5248-103">Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.</span><span class="sxs-lookup"><span data-stu-id="b5248-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="b5248-104">**Registru cheie**</span><span class="sxs-lookup"><span data-stu-id="b5248-104">**Registry key**</span></span>|<span data-ttu-id="b5248-105">\*\*Tastați \*\*</span><span class="sxs-lookup"><span data-stu-id="b5248-105">**Type**</span></span>|<span data-ttu-id="b5248-106">**Valoare**</span><span class="sxs-lookup"><span data-stu-id="b5248-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b5248-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b5248-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b5248-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b5248-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b5248-109">1</span><span class="sxs-lookup"><span data-stu-id="b5248-109">1</span></span>  <br/> |
   
<span data-ttu-id="b5248-110">Pentru informaţii suplimentare, consultaţi [Permite autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b5248-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b5248-p101">Monica este activată în mod implicit în Office 365 ProPlus şi Office 2016. > Servicii remote Desktop (RDS) a fost numit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="b5248-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

