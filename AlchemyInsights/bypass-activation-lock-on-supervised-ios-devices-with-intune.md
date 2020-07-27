---
title: Bypass blocare de activare pe dispozitivele iOS supravegheate cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424215"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bypass blocare de activare pe dispozitivele iOS supravegheate cu Intune

Capacitatea de a ocoli blocarea de activare pe dispozitivele iOS face mai ușor de recuperat din scenariul în care un utilizator permite blocarea de activare pe un dispozitiv corporativ, și apoi părăsește compania.

Cerințele prealabile pentru a ocoli o blocare de activare includ:

- Un dispozitiv este "supravegheat".
- Blocarea activării este activată cu succes utilizând politica de restricționare a dispozitivului iOS în Intune.

În plus, atunci când ocoliți o blocare de activare, ar trebui:

- Posedă fizic dispozitivul fiind șters.
- Copiați codul înainte de a emite ștergerea.

**Notă:** Codul de ștergere nu este sensibil la litere mari și mici, astfel încât caracterele "-" nu sunt necesare.

Pentru detalii, consultați [Blocarea de activare bypass pe dispozitivele iOS supravegheate cu Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**ÎNTREBĂRI FRECVENTE**

Î: **Am emis o acțiune la distanță pentru a elimina datele companiei de pe un dispozitiv, iar acum este blocat într-o stare în așteptare.**

R: Pentru ca o acțiune la distanță să se finalizeze cu succes, dispozitivul vizat trebuie să fie online și sănătos. În următoarele situații, acțiunea la distanță rămâne într-o stare în așteptare timp de 30 de zile sau până când dispozitivul recunoaște comanda atunci când dispozitivul:

- Nu are conectivitate.
- Își pierde statutul de management cu Intune.

Dacă credeți că un dispozitiv nu se mai face check-in și că nu va elimina datele companiei, selectați Ștergere. Ștergerea elimină înregistrarea dispozitivului, astfel încât să nu mai apară în lista de dispozitive Intune. Pentru ca dispozitivul să devină din nou activ, utilizatorul trebuie să reînscrie dispozitivul.

Î: **De ce anumite acțiuni la distanță nu sunt disponibile pentru mine?**

R: Nu toate platformele acceptă toate acțiunile dispozitivelor la distanță. Următoarele acțiuni la distanță sunt specifice platformei.

- Blocare activare bypass (numai iOS)
- Pornire proaspătă (numai windows)
- Mod pierdut (numai iOS)
- Localizare dispozitiv (numai iOS)
- Repornire (numai Windows)

Pentru mai multe detalii despre fiecare acțiune, consultați [Acțiunile disponibile ale dispozitivului](https://docs.microsoft.com/intune/device-management#available-device-actions).