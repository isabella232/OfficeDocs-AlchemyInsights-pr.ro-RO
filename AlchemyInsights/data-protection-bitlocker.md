---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731251"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptării BitLocker cu Intune

 Politica de protecție a Endpoint-ului Intune poate fi utilizată pentru a configura setările de criptare BitLocker pentru dispozitivele Windows. Pentru mai multe informații, consultați [Setări Windows 10 (și versiuni mai recente) pentru a proteja dispozitivele utilizând Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Trebuie să rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker, care este declanșată fără aplicarea politicii MDM. Acest lucru poate avea un impact asupra aplicării politicii dacă sunt configurate setările non-implicite. Consultați următoarele întrebări frecvente pentru mai multe detalii.
 
Pentru informații despre depanarea problemelor cu BitLocker, consultați [Depanarea politicilor BitLocker în Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**ÎNTREBĂRI FRECVENTE**

 Î: ce ediții de Windows acceptă criptarea dispozitivelor folosind Politica de protecție a Endpoint?<br>
 A: Politica de protecție a Endpoint-ului setări din Intune este implementată utilizând CSP-ul [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nu toate edițiile sau compilările Windows acceptă CSP-ul BitLocker. <br><br>
      În acest moment, sunt acceptate următoarele ediții Windows: Enterprise, Education, mobile, Enterprise mobile și Professional (compilarea 1809 și versiuni mai recente).
 
Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite de sistem de operare pentru metoda de criptare și tăria cifră (XTS-AES-128), va aplica o politică cu setări diferite care declanșează automat recriptarea unității cu noile setări?<br>
R: Nu. Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.<br><br>
**Notă:** Pentru dispozitivele care se înscriu cu autopilot, criptarea automată care va apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite utilizarea setărilor bazate pe politică în locul valorilor implicite pentru sistemul de operare.
 
Î: dacă un dispozitiv este criptat ca rezultat al aplicării politicii Intune, acesta va fi decriptat atunci când se elimină Politica?<br>
A: eliminarea politicii legate de criptare nu determină decriptarea unităților care au fost configurate.
 
Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are BitLocker activat, chiar dacă este?<br>
A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeazã clientul de atestare a sanatatii dispozitivelor Windows (DHA). Acest client măsoară doar starea dispozitivului în timpul încărcării. Așadar, dacă un dispozitiv nu a fost repornit de când s-a finalizat criptarea BitLocker, serviciul client DHA nu va raporta BitLocker ca fiind activ.
 
 