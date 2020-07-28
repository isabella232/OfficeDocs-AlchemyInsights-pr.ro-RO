---
title: Localizarea dispozitivelor iOS pierdute cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440426"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Localizarea dispozitivelor iOS pierdute cu Intune

Activarea modului pierdut pe un dispozitiv iOS permite unui administrator să aibă un mesaj și un număr de telefon de contact afișat pe ecranul de blocare.

După activarea modului pierdut, administratorul poate utiliza acțiunea Localizare dispozitiv pentru a identifica locația fizică a dispozitivului.

Acțiunea Localizare dispozitiv din Intune funcționează cu dispozitive iOS pentru a afișa locația unui anumit dispozitiv pe o hartă.

Utilizarea acestei acțiuni necesită ca dispozitivul iOS să fie în:

- Mod supravegheat
- Mod pierdut

Pentru mai multe informații, consultați [Activarea modului pierdut pe dispozitivele iOS/iPadOS cu Intune](https://docs.microsoft.com/intune/device-lost-mode) și [Locate dispozitive iOS/iPadOS pierdute sau furate cu Intune](https://docs.microsoft.com/intune/device-locate).

**ÎNTREBĂRI FRECVENTE**

Î: Am emis o acțiune la distanță pentru a elimina datele companiei de pe un dispozitiv, iar acum este blocat într-o stare în așteptare.

R: Pentru ca o acțiune la distanță să se finalizeze cu succes, dispozitivul vizat trebuie să fie online și sănătos. În următoarele situații, acțiunea la distanță rămâne într-o stare în așteptare timp de 30 de zile sau până când dispozitivul recunoaște comanda:

- Când dispozitivul nu are conectivitate
- Când dispozitivul își pierde starea de gestionare cu Intune

Dacă credeți că un dispozitiv nu se mai face check-in și că nu va putea elimina datele companiei, selectați Ștergere. Ștergerea elimină înregistrarea dispozitivului, astfel încât să nu mai apară în lista de dispozitive Intune. Dacă dispozitivul devine activ din nou, utilizatorul său va trebui să-l reînscrie.

Î: De ce anumite acțiuni la distanță nu sunt disponibile pentru mine?

R: Nu toate platformele acceptă toate acțiunile dispozitivelor la distanță. Următoarele acțiuni la distanță sunt specifice platformei, astfel încât acestea sunt disponibile numai pentru platformele menționate.

- Blocare activare bypass (numai iOS)
- Pornire proaspătă (numai windows)
- Mod pierdut (numai iOS)
- Localizare dispozitiv (numai iOS)
- Repornire (numai Windows)

Pentru mai multe detalii despre fiecare acțiune, consultați [Acțiunile disponibile ale dispozitivului](https://docs.microsoft.com/intune/device-management#available-device-actions).