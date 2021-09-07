---
title: Manager Punct final - Niveluri de referință pentru securitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923566"
---
# <a name="endpoint-manager---security-baselines"></a>Manager Punct final - Niveluri de referință pentru securitate

Nivelurile de referință pentru securitate sunt grupuri preconfigurate de setări Windows care vă ajută să aplicați setările de securitate recomandate de echipele de securitate relevante. Aceste niveluri de referințe pot fi particularizate pentru a livra doar setările și valorile dorite. Pentru mai multe informații despre nivelurile de referință pentru securitate, consultați [Utilizați niveluri de referință pentru securitate pentru a configura dispozitivele Windows 10 în Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Există niveluri de referință pentru aceste produse:

- Setări de securitate MDM Windows
- Microsoft Defender pentru securitate Punct final
- Microsoft Edge

Fiecare dintre nivelurile de referință este actualizat periodic și lansat în versiuni incrementale. Fiecare versiune adaugă și elimină setările din versiunea anterioară, pentru a se asigura că nivelul de referință îndeplinește instrucțiunile actuale. Consola cu niveluri de referință de securitate din Securitatea punctului final permite compararea diferitelor versiuni, făcând vizibile modificările de la o versiune la alta.

Pentru instrucțiuni despre cum să modificați eficient versiunea nivelului de referință implementată, consultați [Gestionarea profilurilor privind nivelul de referință de securitate în Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

După implementarea unui nivel de referință pentru securitate, puteți monitoriza starea setărilor de implementare și revizuire pe o bază de dispozitiv.

Deoarece nivelurile de referință de securitate conțin multe setări, este important să revizuiți modificările de configurare și să efectuați testarea pentru a vă asigura că toate setările sunt potrivite pentru dispozitivele și necesitățile dvs. de afaceri.

**Notă:** Datele de raportare pentru nivelurile de referință pot dura până la 24 de ore pentru a apărea de la implementarea inițială pe un dispozitiv și până la 6 ore pentru actualizări suplimentare. 

Cauza cea mai comună a neaplicării unei setări a nivelului de referință este faptul că aceeași setare este utilizată în alt profil. Acest scenariu poate fi investigat pentru un anumit dispozitiv selectând acel dispozitiv din nodul Stare dispozitiv al profilului Nivel de referință pentru securitate. Pentru detalii, consultați [Soluționarea conflictelor privind referințele pentru securitate](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).