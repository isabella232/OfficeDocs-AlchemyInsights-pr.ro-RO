---
title: Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793892"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive

Nivelurile de referință de securitate Intune contribuie la protejarea utilizatorilor și a dispozitivelor. Referințele de Windows sunt grupurile preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valorile implicite recomandate de echipele de securitate relevante. Creând un profil de referință de securitate în Intune, creați un șablon care constă în mai multe profiluri de configurare a dispozitivului.

Atunci când implementați niveluri de referință de securitate pentru grupuri de utilizatori sau dispozitive, setările se aplică pentru dispozitivele care rulează pe dispozitivele Windows 10 sau mai recente. De exemplu, nivelul de referință de securitate MDM (mobile device management) Microsoft activează automat BitLocker pentru unitățile amovibile, necesită parola pentru deblocarea unui dispozitiv și dezactivează autentificarea de bază. Atunci când o valoare implicită nu funcționează pentru mediul dvs., puteți particulariza nivelul de referință pentru a aplica setările de care aveți nevoie.

De asemenea, referințele de securitate vă ajută să stabiliți un flux de lucru securizat end-to-end Microsoft 365. Un nivel de referință de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea. Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based solid guidance and extensive experience.

Dacă nu sunteți sigur de unde să începeți, nivelurile de referință de securitate vă ajută să creați și să implementați rapid un profil sigur. Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai ușoară cu nivelurile de referință de securitate, deoarece acestea sunt încorporate în Intune și includ capacități de gestionare de ultimă oră.

Pentru a afla mai multe, [consultați Referințe Windows securitate și](/windows/security/threat-protection/windows-security-baselines) Gestionarea [dispozitivelor mobile.](/windows/client-management/mdm/)

