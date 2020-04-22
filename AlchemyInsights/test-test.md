---
title: Termeni care lipsesc din Depozitul de termeni SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766865"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptării Bitlocker cu Intune

Intune Endpoint Protection Policy poate fi utilizat pentru a configura setările de criptare Boitlocker pentru dispozitiveLe Windows, așa este descris în: Setări Windows10 (și versiuni ulterioare) pentru a proteja dispozitivele utilizând Intune

Ar trebui să fie conștienți de faptul că multe dispozitive mai noi care execută Windows 10 acceptă criptarea automată bitlocker care se declanșează fără aplicarea politicii MDM. Acest lucru poate avea impact asupra aplicării politicii dacă sunt configurate setările neimplicite. Consultați Întrebări frecvente pentru mai multe detalii.


Faq  Î: Ce ediții de criptare dispozitiv de asistență Windows utilizând Politica de protecție Endpoint?
 R: Setările din Intune Endpoint Protection Policy sunt implementate utilizând Bitlocker CSP.Nu toate edițiile, nici compilările de Windows acceptă Bitlocker CSP. 
      În acest moment Edițiile Windows: Enterprise; Sunt acceptate educația, mobilul, întreprinderea mobilă și profesioniștii (începând cu versiunea 1809).




Î: Dacă un dispozitiv este deja criptat cu Bitlocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea de criptare (XTS-AES-128) aplicarea unei politici cu setări diferite declanșează automat recriptarea unității cu noile setări?

R: Nu. Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.

Notă Pentru dispozitivele înscrise cu Autopilot criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite setările bazate pe politică pentru a fi utilizate în loc de valori implicite os




Q Dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune va fi decriptat atunci când această politică este eliminat?

R: Eliminarea politicii legate de criptare NU duce la decriptarea unităților care au fost configurate.




Î: De ce politica de conformitate intune arată că dispozitivul meu nu are "Bitlocker Activat", dar este?

R: Setarea "Bitlocker activat" în politica de conformitate intune utilizează clientul Windows Device Health Atestare (DHA). Acest client măsoară numai starea dispozitivului la momentul pornire. Deci, dacă un dispozitiv nu a fost repornit, deoarece criptarebitlocker a fost finalizat serviciul client DHA nu va raporta bitlocker ca fiind activ.