---
title: Inventar dispozitiv Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440474"
---
# <a name="intune-device-inventory"></a>Inventar dispozitiv Intune

Lama Devices oferă administratorului o perspectivă asupra dispozitivelor aflate în administrare în Intune pe bază de dispozitiv. Informațiile afișate includ: Hardware, Aplicații descoperite, Starea de conformitate a dispozitivului și Starea configurației dispozitivului.

Datele de inventar pentru hardware și aplicațiile descoperite sunt colectate pe un ciclu de șapte zile. Aplicațiile și elementele specifice ale hardware-ului raportate diferă în funcție de sistemul de operare al dispozitivului și dacă dispozitivul este deținut personal sau de companie.

Pentru mai multe informații, consultați [Vedeți detaliile dispozitivului în Intune](https://docs.microsoft.com/intune/device-inventory).

**ÎNTREBĂRI FRECVENTE**

Î: Nu primesc o listă completă de inventar a aplicațiilor prezente pe dispozitivele Windows încorporate intune. de ce nu?

R: În acest moment, numai aplicațiile moderne sunt listate pentru PC-urile Windows 10 care sunt identificate ca dispozitive corporative. Intune nu colectează informații despre aplicațiile Win32 instalate pe aceste dispozitive.

Î: De ce numerele de telefon nu sunt colectate de pe toate dispozitivele?

R: Telefoanele clasificate ca dispozitive corporative în Intune nu sunt identificate cu numărul lor de telefon complet atunci când, de exemplu, executați un raport de inventar al dispozitivului mobil. Numerele de telefon ale dispozitivului Bring-you-own sunt întotdeauna parțial mascate cu asteriscuri (****) și afișează doar ultimele patru cifre.