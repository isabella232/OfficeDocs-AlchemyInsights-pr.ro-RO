---
title: Starea senzorului pentru punctul final Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676339"
---
# <a name="defender-endpoint-check-sensor-status"></a>Starea senzorului pentru punctul final Defender

Dala **Dispozitive cu probleme de** senzor se află pe tabloul de bord Operațiuni de securitate. Această dală furnizează informații despre capacitatea dispozitivului individual de a furniza date despre senzor și de a comunica cu serviciul Defender pentru puncte finale. Acesta raportează câte dispozitive necesită atenție și vă ajută să identificați dispozitivele problematice și să luați măsuri pentru a corecta problemele cunoscute.

Doi indicatori de stare ai dalei furnizează informații despre numărul de dispozitive care nu raportează corect serviciul:

- **Configurați greșit** Dispozitivele care pot fi parțial de raportare a datelor despre senzor la serviciul Defender pentru punctul final și care pot avea erori de configurare care trebuie corectate.
- **Inactiv** Dispozitivele care au oprit raportarea la serviciul Defender pentru puncte finale mai mult de șapte zile în ultima lună.

Un clic pe oricare dintre grupuri vă direcționează către lista Dispozitive, filtrată după opțiunile dvs. În lista Dispozitive, puteți filtra lista cu starea de bună stare după următoarea stare:

- **Activ** Dispozitive care raportează în mod activ la serviciul Defender pentru puncte finale.
- **Configurați greșit** Dispozitivele care pot fi parțial de raportare a datelor despre senzor la serviciul Defender pentru punctul final, dar au erori de configurare care trebuie corectate. Dispozitivele configurate greșit pot avea una sau o combinație a următoarelor probleme:

    - Fără date despre senzor - Dispozitivele nu mai trimit date despre senzor. Avertizările limitate se pot declanșa de pe dispozitiv.
    - Comunicații cu deficiențe - Capacitatea de a comunica cu dispozitivul este afectată. Trimiterea de fișiere pentru analiză aprofundată, blocarea fișierelor, blocarea dispozitivului din rețea și alte acțiuni care necesită comunicarea cu dispozitivul pot să nu funcționează.
- **Inactiv** Dispozitivele care au oprit raportarea la serviciul Defender pentru punct final.

Puteți descărca întreaga listă în format CSV utilizând caracteristica Export.

Pentru mai multe informații, consultați [Verificarea stării stării senzorului în Microsoft Defender pentru punctul final.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Pentru mai multe informații despre cauza inactivă sau configurarea greșită a unui dispozitiv, consultați Remedierea senzorilor ne sănătos în [Microsoft Defender pentru punctul final.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
