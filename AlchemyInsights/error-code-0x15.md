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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Eroare în timpul activării Office 2013 pe servicii Desktop la distanță

Dacă primiți o eroare la activarea Office 2013 pe implementări de servicii Desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.
  
|**Cheie de registry**|**Tip**|**Valoarea**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Pentru mai multe informații, consultați [Activarea autentificării moderne pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL este activat în mod implicit în Microsoft 365 Apps pentru întreprinderi și Office 2016. Servicii Desktop la distanță (RDS) a fost denumit anterior Terminal Services.
  