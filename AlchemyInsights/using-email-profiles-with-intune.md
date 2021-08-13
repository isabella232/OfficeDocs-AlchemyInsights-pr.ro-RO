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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919435"
---
# <a name="using-email-profiles-with-intune"></a>Utilizarea profilurilor de e-mail cu Intune

Intune poate fi utilizat pentru a crea și a implementa profiluri de e-mail pentru clientul de e-mail nativ (predefinit) pe mai multe platforme de dispozitive.

Pentru informații despre unele dintre restricțiile asociate cu profilurile de e-mail, inclusiv despre modul în care sunt gestionate prezența profilurilor existente și despre cum să eliminați profilurile de e-mail, consultați Adăugarea setărilor de e-mail la dispozitivele care utilizează [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Pentru mai multe informații despre cum să creați profiluri de e-mail pentru fiecare platformă de dispozitiv, consultați:

[Setările dispozitivului Android pentru a configura e-mailul, autentificarea și sincronizarea în Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Adăugați setări de e-mail pentru dispozitive iOS și iPadOS în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Setările de profil de e-Microsoft Intune de e-mail pentru dispozitivele care Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Setările de profil de e-mail pentru dispozitivele care Windows 10 în Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problemă comună de sincronizare**

**Un KNOX pe profilul de e-mail Android împiedică sincronizarea cu dispozitivele de utilizator Contacte, Calendar și Activități.**

KNOX pe profilul de e-mail Android KNOX oferă administratorului opțiunea de a decide ce tipuri de conținut sunt sincronizate cu dispozitivul, setând-o pe fiecare la activat.

Dacă setarea pentru oricare dintre tipurile de conținut este setată la **Neconfigurat** (implicit), acel tip de conținut nu se sincronizează automat. Un utilizator poate activa tipul de conținut dorit direct pe dispozitiv, dar configurația respectivă este suprascrisă de setarea de politică Intune și sincronizarea se oprește pentru acel tip de conținut.

