---
title: Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573533"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10

Liniile de referință de securitate Intune ajută la protejarea utilizatorilor și dispozitivelor. Liniile de referință de securitate sunt grupuri de setări Windows preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valori implicite recomandate de echipele de securitate relevante. Prin crearea unui profil de referință de securitate în Intune, creați un șablon care constă din mai multe profiluri de configurare a dispozitivelor.

Atunci când implementați linii de referință de securitate la grupuri de utilizatori sau dispozitive, setările se aplică la dispozitivele care rulează în Windows 10 sau o versiune mai recentă. De exemplu, linie de bază de securitate MDM automat (1) activează BitLocker pentru unitățile amovibile, (2) necesită parola pentru deblocarea unui dispozitiv și (3) dezactivează autentificarea de bază. Atunci când o valoare implicită nu funcționează pentru mediul dvs., particularizați valoarea de referință pentru a aplica setările de care aveți nevoie.

De asemenea, liniile de referință de securitate vă ajută să stabiliți un flux de lucru securizat final în Microsoft 365. Iată câteva dintre următoarele avantaje:

- O linie de bază de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea. Deoarece Intune parteneri cu echipa de securitate Windows care creează valori de referință pentru politicile de grup, aceste recomandări se bazează pe orientări solide și o experiență extinsă.
- Dacă nu sunteți familiarizat cu Intune și nu sunteți sigur de unde să începeți, atunci liniile de referință de securitate vă vor ajuta să creați și să implementați rapid un profil securizat.
- Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai simplă cu liniile de bază de securitate, deoarece acestea sunt încorporate în Intune și includ capacități de vârf pentru gestionare.

Pentru a afla mai multe, consultați [liniile de bază de securitate Windows](https://go.microsoft.com/fwlink/?linkid=2141503) și [gestionarea dispozitivelor mobile](https://go.microsoft.com/fwlink/?linkid=2141701).