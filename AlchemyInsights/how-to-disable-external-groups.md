---
title: Cum se dezactivează grupurile externe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015632"
---
# <a name="how-to-disable-external-groups"></a>Cum se dezactivează grupurile externe

Yammer mesajele externe aplică Exchange de transport (ERS), un set de controale proactive care împiedică partajate informațiile firmei. Pentru a restricționa crearea de grupuri externe pentru utilizatori, trebuie să configurați o regulă de transport Exchange (ETR) și apoi să configurați Yammer pentru a utiliza regula de transport Exchange pentru a bloca mesageria externă.
  
După ce ați creat o regulă în centrul Exchange Online de administrare, urmați acești pași pentru a seta ca ETR să se aplice Yammer:
  
- Conectați-vă la Yammer ca administrator verificat și, în centrul **Yammer,** accesați C Content **and Security security \> Setări.**

- Sub **Mesagerie externă, selectați** **Impuneți regulile Exchange Online Exchange de transport (ERS) în Yammer.**

- Alegeți **Salvare.**

Pentru mai multe informații, consultați [Dezactivarea mesageriei externe într-o Yammer date.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  