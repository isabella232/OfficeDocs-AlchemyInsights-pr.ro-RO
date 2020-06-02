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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Eroare în timpul activării Office 2013 pe servicii Desktop la distanță

Dacă primiți o eroare la activarea Office 2013 pe implementări de servicii Desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.
  
|**Cheie de registry**|**Tip**|**Valoarea**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Pentru mai multe informații, consultați [Activarea autentificării moderne pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL este activat în mod implicit în Microsoft 365 Apps pentru întreprinderi și Office 2016. Servicii Desktop la distanță (RDS) a fost denumit anterior Terminal Services.
  