---
title: se dezactivează grupuri externe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720780"
---
# <a name="how-to-disable-external-groups"></a>se dezactivează grupuri externe

Yammer mesagerie externă aplică Reguli de transport Exchange (ETRs), un set de controale proactive pentru a preveni informațiile companiei de a fi partajate. Pentru a restricționa utilizatorii să creeze grupuri externe, trebuie să configurați o regulă de transport Exchange (ETR), și apoi configurați Yammer pentru a utiliza regula Exchange Transport pentru a bloca mesageria externă.
  
După ce ați creat o regulă în centrul de administrare Exchange Online, urmați acești pași pentru a seta ETR să se aplice în Yammer:
  
- Faceți Log on la Yammer ca administrator verificat, iar în **centrul de administrare Yammer**, accesați **C Setări de securitate conținut și securitate. \> **

- Sub **Mesagerie externă**, **selectați Impuneți regulile de transport Exchange Online Exchange (ETRs) în Yammer.**

- Alegeți **Salvare**.

Pentru mai multe informații, consultați [Dezactivarea mesageriei externe într-o rețea Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  