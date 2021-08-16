---
title: Inventar dispozitiv Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014084"
---
# <a name="intune-device-inventory"></a>Inventar dispozitiv Intune

Sistemul blade Dispozitive furnizează detaliile administratorului asupra dispozitivelor aflate în gestionare în Intune pe fiecare dispozitiv. Informațiile afișate includ: Hardware, aplicații descoperite, starea de conformitate a dispozitivului și starea de Configurare dispozitiv.

Datele inventarului pentru hardware și aplicațiile descoperite sunt colectate într-un ciclu de șapte zile. Aplicațiile și elementele specifice ale hardware-ului raportate diferă în funcție de sistemul de operare al dispozitivului și de proprietarul personal sau corporativ al dispozitivului.

Pentru mai multe informații, consultați [Vedeți detaliile dispozitivului în Intune](https://docs.microsoft.com/intune/device-inventory).

**ÎNTREBĂRI FRECVENTE**

Î: Nu primesc o listă completă de inventar cu aplicațiile prezente pe dispozitivele mele cu Windows Intune. de ce nu?

A: În acest moment, doar aplicațiile moderne sunt listate pentru Windows 10 PC-uri care sunt identificate ca dispozitive de corporație. Intune nu colectează informații despre aplicațiile Win32 instalate pe aceste dispozitive.

Î: De ce nu sunt colectate numerele de telefon de pe toate dispozitivele?

A: Telefoanele clasificate ca dispozitive de corporație în Intune nu sunt identificate cu numărul lor de telefon complet atunci când, de exemplu, rulați un raport de inventar pentru dispozitive mobile. Numerele de telefon de tip Aducere pe propriul dispozitiv sunt întotdeauna mascate parțial cu asteriscuri (****) și afișează numai ultimele patru cifre.