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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527046"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Eroare la activarea Office 2013 pe Remote Desktop servicii

Dacă primiţi o eroare în timp ce activarea Office 2013 pe implementările de Remote Desktop Services (RDS), ia în considerare să permită ADAL editarea registry-ului.
  
|**Registru cheie**|**Tip**|**Valoarea**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Pentru informaţii suplimentare, consultaţi [Permite autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Monica este activată în mod implicit în Office 365 ProPlus şi Office 2016. Remote Desktop servicii (RDS) a fost numit anterior Terminal Services.
  