---
title: Termeni lipsă din SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053525"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptare BitLocker cu Intune

Politica de protecție Intune Endpoint poate fi utilizată pentru a configura setările de criptare Boitlocker pentru dispozitivele Windows, așa este descris în: Windows10 (și versiunile ulterioare) pentru a proteja dispozitivele utilizând Intune

Trebuie să știți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată a BitLocker care este declanșată fără aplicarea politicii MDM. Acest lucru poate afecta aplicarea politicii dacă nu sunt configurate setări implicite. Consultați întrebări frecvente pentru mai multe detalii.


Întrebări  frecvente: ce ediții de criptare dispozitiv de suport Windows utilizând politica de protecție Endpoint?
 A: setările în Intune Endpoint Protection politica sunt implementate utilizând CSP-ul BitLocker.Nu toate edițiile și nici compilările de Windows acceptă CSP-ul BitLocker. 
      În acest moment Windows Editions: Enterprise; Educație, mobile, Mobile Enterprise și Professional (de la Build 1809 începând) sunt suportate.




Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128) va aplica o politică cu diferite setări declanșează automat re-criptarea unității cu noile setări?

A: nu. Pentru a aplica noile setări de cifrare, unitatea trebuie decriptată mai întâi.

Notă pentru dispozitivele care se înscriu cu autopilot criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată care permite setările de politică bazate pentru a fi utilizate în locul implicite de sistem de operare




Q dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune va fi decriptat atunci când această politică este eliminată?

A: eliminarea politicii legate de criptare nu duce la decriptarea unităților care au fost configurate.




Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are "BitLocker enabled", dar este?

A: setarea "BitLocker enabled" în Politica de conformitate Intune utilizeaza clientul Windows Device sănătate Atestation (DHA). Acest client măsoară numai starea dispozitivului la Boot Time. Deci, dacă un dispozitiv nu a fost repornit deoarece criptare BitLocker s-a finalizat serviciul de client DHA nu va raporta BitLocker ca fiind activ.