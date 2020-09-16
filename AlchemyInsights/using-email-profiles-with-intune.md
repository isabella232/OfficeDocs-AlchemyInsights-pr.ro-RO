---
title: Utilizarea profilurilor de e-mail cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653300"
---
# <a name="using-email-profiles-with-intune"></a>Utilizarea profilurilor de e-mail cu Intune

Intune poate fi utilizat pentru a crea și implementa profiluri de e-mail pentru clientul de e-mail nativ (încorporat) de pe mai multe platforme de dispozitive.

Pentru informații despre unele dintre restricțiile asociate cu profilurile de e-mail, inclusiv despre modul în care sunt gestionate prezența profilurilor existente și cum să eliminați profilurile de e-mail, consultați [adăugarea setărilor de e-mail la dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/email-settings-configure).

Pentru mai multe informații despre cum să creați profiluri de e-mail pentru fiecare platformă de dispozitive, consultați:

[Setări dispozitiv Android pentru a configura e-mailul, autentificarea și sincronizarea în Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adăugarea setărilor de e-mail pentru dispozitive iOS și iPadOS în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Setările de profil de e-mail din Microsoft Intune pentru dispozitivele care execută Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Setările de profil de e-mail pentru dispozitivele care execută Windows 10 în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problemă de sincronizare obișnuită**

**Un KNOX din profilul de e-mail Android previne persoanele de contact, calendarul și activitățile de utilizator, de la sincronizarea la dispozitivele de utilizator.**

Profilul de e-mail KNOX din Android KNOX oferă administratorului opțiunea de a decide ce tipuri de conținut sunt sincronizate cu dispozitivul setând fiecare la activat.

Dacă setarea pentru oricare dintre tipurile de conținut este setată la **neconfigurat** (implicit), acel tip de conținut nu se sincronizează automat. Un utilizator poate activa tipul de conținut pe care îl doresc direct pe dispozitiv, dar acea configurație este suprascrisă de setarea de politică Intune, iar sincronizarea se oprește pentru acel tip de conținut.

