---
title: Utilizarea profilurilor de e-mail cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555247"
---
# <a name="using-email-profiles-with-intune"></a>Utilizarea profilurilor de e-mail cu Intune

Intune poate fi utilizat pentru a crea și implementa profiluri de e-mail pentru clientul de e-mail nativ (încorporat) pe mai multe platforme de dispozitive.

Pentru informații despre unele dintre restricțiile asociate profilurilor de e-mail, inclusiv modul în care sunt gestionate prezența profilurilor existente și modul de eliminare a profilurilor de e-mail, consultați [Adăugarea setărilor de e-mail la dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/email-settings-configure).

Pentru mai multe informații despre să creați profiluri de e-mail pentru fiecare platformă de dispozitive, consultați:

[Setările dispozitivului Android pentru configurarea e-mailului, a autentificării și a sincronizării în Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adăugarea setărilor de poștă electronică pentru dispozitivele iOS și iPadOS în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Setările profilului de e-mail în Microsoft Intune pentru dispozitivele care rulează Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Setări profil de e-mail pentru dispozitivele care rulează Windows 10 în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problemă comună de sincronizare**

**Un profil de e-mail KNOX pe Android împiedică contactele, calendarul și activitățile utilizatorilor să fie sincronizate cu dispozitivele de utilizator.**

Profilul de e-mail KNOX on Android KNOX oferă administratorului opțiunea de a decide ce tipuri de conținut sunt sincronizate cu dispozitivul, setând fiecare la activat.

Dacă setarea pentru oricare dintre tipurile de conținut este setată la **Neconfigurat** (implicit), acel tip de conținut nu se sincronizează automat. Un utilizator poate activa manual tipul de conținut dorit direct pe dispozitiv, dar această configurație este suprascrisă de setarea de politică Intune, iar sincronizarea se oprește pentru acel tip de conținut.

