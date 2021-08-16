---
title: Cod de 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Dacă primiți o eroare în timp ce activați Office 2013 pentru implementările serviciilor desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100774"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Eroare în timpul Office 2013 pe Servicii desktop la distanță

Dacă primiți o eroare în timp ce activați Office 2013 pentru implementările serviciilor desktop la distanță (RDS), luați în considerare activarea ADAL prin editarea registry.
  
|**Cheie de registry**|**Tip**|**Valoare**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Pentru mai multe informații, [consultați Activarea autentificării moderne pentru Office 2013 pe Windows dispozitive .](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL este activat în mod implicit în Aplicații Microsoft 365 pentru întreprindere și Office 2016. Serviciile desktop la distanță (RDS) au fost denumite anterior Terminal Services.
  