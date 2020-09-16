---
title: Condiții lipsă din depozitul de termeni SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750463"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptării BitLocker cu Intune

Politica de protecție a Endpoint-ului Intune poate fi utilizată pentru a configura setările de criptare Boitlocker pentru dispozitivele Windows, așa cum este descris în: Windows10 (și versiuni mai recente) pentru a proteja dispozitivele utilizând Intune

Trebuie să rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker care este declanșată fără aplicarea politicii MDM. Acest lucru poate avea un impact asupra aplicării politicii dacă sunt configurate setările non-implicite. Consultați întrebări frecvente pentru mai multe detalii.


Întrebări frecvente   î: ce ediții de criptare a dispozitivelor de asistență Windows utilizând politica de protecție pentru Endpoint?
 A: Politica de protecție a Endpoint-ului setări din Intune este implementată utilizând CSP-ul BitLocker.Nu toate edițiile și versiunile de Windows acceptă CSP-ul BitLocker. 
      În acest moment edițiile Windows: Enterprise; Sunt acceptate educația, telefonul mobil, întreprinderea mobilă și Professional (de la compilarea 1809 începând cu).




Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite de sistem de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128) va aplica o politică cu setări diferite, declanșând automat recriptarea unității cu noile setări?

R: Nu. Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.

Notă pentru dispozitivele care se înscriu cu autopilot, criptarea automată care va apărea în timpul OOBE nu se declanșează până când politica Intune este evaluată, care permite ca setările bazate pe politică să fie utilizate în locul valorilor implicite pentru sistemul de operare




Î dacă un dispozitiv este criptat ca rezultat al aplicării politicii Intune, acesta va fi decriptat atunci când se elimină Politica?

A: eliminarea politicii legate de criptare nu determină decriptarea unităților care au fost configurate.




Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are "BitLocker activat", dar este?

A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeazã clientul de atestare a sanatatii dispozitivelor Windows (DHA). Acest client măsoară doar starea dispozitivului în timpul încărcării. Așadar, dacă un dispozitiv nu a fost repornit, deoarece criptarea BitLocker a fost finalizată, serviciul client DHA nu va raporta BitLocker ca fiind activ.