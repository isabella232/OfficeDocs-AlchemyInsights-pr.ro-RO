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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929101"
---
<span data-ttu-id="cb962-103">Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.</span><span class="sxs-lookup"><span data-stu-id="cb962-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="cb962-104">**Registru cheie**</span><span class="sxs-lookup"><span data-stu-id="cb962-104">**Registry key**</span></span>|<span data-ttu-id="cb962-105">\*\*Tastați \*\*</span><span class="sxs-lookup"><span data-stu-id="cb962-105">**Type**</span></span>|<span data-ttu-id="cb962-106">**Valoare**</span><span class="sxs-lookup"><span data-stu-id="cb962-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cb962-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="cb962-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="cb962-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="cb962-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="cb962-109">1</span><span class="sxs-lookup"><span data-stu-id="cb962-109">1</span></span>  <br/> |
   
<span data-ttu-id="cb962-110">Pentru informaţii suplimentare, consultaţi [Permite autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="cb962-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="cb962-p101">Monica este activată în mod implicit în Office 365 ProPlus şi Office 2016. > remote Desktop servicii (RDS) a fost numit anterior Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="cb962-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

