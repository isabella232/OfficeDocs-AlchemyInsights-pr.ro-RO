---
title: EndPoint Manager - Referințe de securitate
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421088"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Referințe de securitate

Nivelurile de referință de securitate sunt grupuri preconfigurate de setări Windows care vă ajută să aplicați setările de securitate recomandate de echipele de securitate relevante. Aceste niveluri de referință pot fi particularizate pentru a livra doar setările și valorile dorite. Pentru mai multe informații despre nivelurile de referință de securitate, consultați Utilizarea nivelurilor de referință de securitate pentru a [configura dispozitivele Windows 10 în Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

În prezent, există niveluri de referință pentru aceste produse:

- Setări Securitate Windows MDM
- Microsoft Defender pentru securitatea punct final
- Microsoft Edge

Fiecare dintre referințe este actualizată periodic și lansată în versiuni incrementale. Fiecare versiune adaugă și sau elimină setările din versiunea anterioară pentru a se asigura că linia de referință îndeplinește instrucțiunile curente. Consola De referință de securitate din Securitatea punctelor finale permite compararea diferitelor versiuni, făcând vizibile modificările de la o versiune la alta.

Pentru instrucțiuni despre cum să modificați cât mai eficient ce versiune de referință este implementată, consultați Gestionarea profilurilor de linie de referință de [securitate în Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

După implementarea unui nivel de referință de securitate, puteți să monitorizați starea implementării și să revizuiți setările pe dispozitive.

**Notă:** Datele de raportare pentru nivelurile de referință pot dura până la 24 de ore pentru a apărea din implementarea inițială pe un dispozitiv și până la 6 ore pentru actualizări suplimentare. 

Cauza cea mai comună a unei setări de referință care nu se aplică este faptul că aceeași setare este utilizată în alt profil. Acest scenariu poate fi investigat pentru un anumit dispozitiv, selectând acel dispozitiv din nodul Stare dispozitiv al profilului de referință de securitate. Pentru detalii, consultați [Rezolvarea conflictelor pentru nivelurile de referință de securitate](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).