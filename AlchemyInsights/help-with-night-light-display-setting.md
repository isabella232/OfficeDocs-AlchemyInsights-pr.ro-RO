---
title: Ajutor pentru setarea pentru afișajul becului de noapte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405178"
---
# <a name="help-with-the-night-light-display-setting"></a>Ajutor pentru setarea pentru afișajul becului de noapte

Pentru a afla mai multe despre setările de afișare pe timp de noapte, [consultați Setarea afișajului pe timp de noapte în Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Dacă opțiunile pentru lumina de noapte sunt estompate în Setări, verificați driverul de afișare: 

1. Faceți clic pe caseta de căutare din bara de activități **și tastați Manager** dispozitive , apoi **selectați Manager dispozitive** în rezultatele de căutare.
1. Extindeți **Plăci video**. 

Din păcate, caracteristica de lumină de noapte nu este disponibilă dacă dispozitivul dvs. utilizează un driver DisplayLink sau un driver de afișare de bază.

Caracteristica lumină de noapte utilizează tehnologia grafică recentă, deci ar putea fi necesar să actualizați driverul de afișare:  

- Căutați actualizări, în Meniul **Pornire**  >  **actualizare setări**&  >  **Securitate**  >  **Windows Update** Căutare  >  **actualizări.**  

SAU

- Vizitați site-ul web de asistență al producătorului de hardware pentru a descărca și instala manual cele mai recente drivere de afișare.

## <a name="reset-night-light-in-the-registry"></a>Resetați lumina de noapte din registry

Dacă actualizarea driverului de afișare nu a funcționat, poate fi necesar să resetați lumina de noapte din registry.  

**Atenție:** Acest pas de depanare este recomandat doar utilizatorilor avansați. Pot apărea probleme grave dacă faceți modificări incorecte în registry. Pentru protecție suplimentară, faceți backup pentru registry înainte de a-l modifica, astfel încât să îl puteți restaura dacă apar probleme.

1. În caseta de căutare, tastați **regedit**, apoi selectați **Registry Editor** în rezultatele căutării.

1. Accesați următoarea cheie de registry: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportați și ștergeți următoarea subcheie:$$windows.data.bluelightreduction.bluelightreductionstate

1. Exportați și ștergeți următoarea subcheie:$$windows.data.bluelightreduction.settings

1. Reporniți Windows și verificați dacă sunt disponibile opțiunile pentru lumina de noapte.


