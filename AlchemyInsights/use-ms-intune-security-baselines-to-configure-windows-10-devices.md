---
title: Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104356"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive

Nivelurile de referință de securitate Intune contribuie la protejarea utilizatorilor și a dispozitivelor. Referințele de securitate Windows grupurile preconfigurate ale setărilor utilizate pentru a aplica un grup cunoscut de setări și valorile implicite recomandate de echipele de securitate relevante. Creând un profil de referință de securitate în Intune, creați un șablon care constă în mai multe profiluri de configurare a dispozitivului.

Atunci când implementați niveluri de referință de securitate pentru grupuri de utilizatori sau dispozitive, setările se aplică pentru dispozitivele care rulează pe dispozitivele Windows 10 sau mai recente. De exemplu, MDM Security Baseline (1) activează BitLocker pentru unitățile amovibile, (2) necesită parola pentru deblocarea unui dispozitiv și (3) dezactivează autentificarea de bază. Atunci când o valoare implicită nu funcționează pentru mediul dvs., particularizați nivelul de referință pentru a aplica setările de care aveți nevoie.

De asemenea, referințele de securitate vă ajută să stabiliți un flux de lucru securizat end-to-end Microsoft 365. Mai jos sunt câteva dintre avantajele acestui lucru:

- Un nivel de referință de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea. Deoarece partenerii Intune cu echipa Windows de securitate care creează niveluri de referință pentru politicile de grup, aceste recomandări se bazează pe îndrumări solide și pe o experiență extinsă.
- Dacă nu sunteți sigur de unde să începeți, nivelurile de referință de securitate vă vor ajuta să creați și să implementați rapid un profil sigur.
- Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai ușoară cu nivelurile de referință de securitate, deoarece acestea sunt încorporate în Intune și includ capacități de ultimă oră pentru gestionare.

Pentru a afla mai multe, [consultați Referințe Windows securitate și](https://go.microsoft.com/fwlink/?linkid=2141503) Gestionarea [dispozitivelor mobile.](https://go.microsoft.com/fwlink/?linkid=2141701)