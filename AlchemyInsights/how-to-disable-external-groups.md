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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704140"
---
# <a name="how-to-disable-external-groups"></a>Cum se dezactivează grupurile externe

Mesageria externă Yammer aplică regulile de transport Exchange (ETRs), un set de controale proactiv pentru a împiedica partajarea informațiilor firmei. Pentru a restricționa utilizatorii să creeze grupuri externe, trebuie să configurați o regulă de transport Exchange (ETR), apoi să configurați Yammer pentru a utiliza regula de transport Exchange pentru a bloca mesageria externă.
  
După ce ați creat o regulă în centrul de administrare Exchange Online, urmați acești pași pentru a seta ETR să se aplice în Yammer:
  
- Conectați-vă la Yammer ca administrator verificat și, în **Centrul de administrare Yammer**, accesați setările C pentru **conținut și \> ** securitate de securitate.

- Sub **Mesagerie externă**, selectați **aplicați regulile de transport Exchange Online Exchange (ETRs) în Yammer.**

- Alegeți **Salvare**.

Pentru mai multe informații, consultați [dezactivarea mesageriei externe într-o rețea Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  