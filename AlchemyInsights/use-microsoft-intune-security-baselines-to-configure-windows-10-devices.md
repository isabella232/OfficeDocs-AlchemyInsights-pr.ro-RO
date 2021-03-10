---
title: Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696379"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Utilizați liniile de bază de securitate Microsoft Intune pentru configurarea dispozitivelor Windows 10

Liniile de referință de securitate Intune ajută la protejarea utilizatorilor și dispozitivelor. Liniile de referință de securitate sunt grupuri de setări Windows preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valori implicite recomandate de echipele de securitate relevante. Prin crearea unui profil de referință de securitate în Intune, creați un șablon care constă din mai multe profiluri de configurare a dispozitivelor.

Atunci când implementați linii de referință de securitate la grupuri de utilizatori sau dispozitive, setările se aplică la dispozitivele care rulează în Windows 10 sau versiuni mai recente. De exemplu, linia de bază de securitate Microsoft Mobile Device Management (MDM) activează automat (1) activează BitLocker pentru unitățile amovibile, (2) necesită parola pentru deblocarea unui dispozitiv și (3) dezactivează autentificarea de bază. Atunci când o valoare implicită nu funcționează pentru mediul dvs., puteți particulariza valoarea de referință pentru a aplica setările de care aveți nevoie.

De asemenea, liniile de referință de securitate vă ajută să stabiliți un flux de lucru securizat final în Microsoft 365. Iată câteva avantaje ale acestei funcționalități:
- O linie de bază de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea. Deoarece Intune parteneri cu echipa de securitate Windows care creează valori de referință pentru politicile de grup, aceste recomandări se bazează pe orientări solide și o experiență extinsă.
- Dacă nu sunteți familiarizat cu Intune și nu sunteți sigur de unde să începeți, atunci liniile de referință de securitate vă vor ajuta să creați și să implementați rapid un profil securizat.
- Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai simplă cu liniile de bază de securitate, deoarece aceste linii de referință de securitate sunt încorporate în Intune și includ capacități de vârf pentru gestionare.

Pentru mai multe informații, consultați [liniile de bază de securitate Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) și [gestionarea dispozitivelor mobile](https://docs.microsoft.com/windows/client-management/mdm/).