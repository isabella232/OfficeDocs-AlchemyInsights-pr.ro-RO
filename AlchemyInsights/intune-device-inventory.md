---
title: Inventarul dispozitivelor Intune
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667890"
---
# <a name="intune-device-inventory"></a>Inventarul dispozitivelor Intune

Lama Devices oferă administratorului informații despre dispozitivele de sub gestionare în Intune pe bază de dispozitiv. Informațiile afișate includ: hardware, aplicații descoperite, starea conformității dispozitivelor și starea configurației dispozitivelor.

Datele de inventar pentru componente hardware și aplicații descoperite sunt colectate pe un ciclu de șapte zile. Aplicațiile și elementele specifice ale componentelor hardware raportate diferă în funcție de sistemul de operare al dispozitivului și dacă dispozitivul este deținut personal sau corporativ.

Pentru mai multe informații, consultați [Vedeți detaliile dispozitivului în Intune](https://docs.microsoft.com/intune/device-inventory).

**ÎNTREBĂRI FRECVENTE**

Î: nu primesc o listă completă de inventar a aplicațiilor prezente pe dispozitivele Windows Intune-inrolat. de ce nu?

A: în acest moment, doar aplicațiile moderne sunt listate pentru PC-urile Windows 10 care sunt identificate ca dispozitive corporative. Intune nu colectează informații despre aplicațiile Win32 instalate pe aceste dispozitive.

Î: de ce nu sunt colectate numerele de telefon de pe toate dispozitivele?

A: telefoanele clasificate ca dispozitive corporative în Intune nu sunt identificate cu numărul de telefon complet atunci când, de exemplu, rulează un raport de inventar al dispozitivelor mobile. Numerele de telefon bring-you-own-dispozitiv sunt întotdeauna parțial mascate cu asteriscuri (* * * *) și afișează doar ultimele patru cifre.