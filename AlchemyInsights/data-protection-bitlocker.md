---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908721"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptare BitLocker cu Intune

 Intune Endpoint Protection politica poate fi utilizat pentru a configura setările de criptare BitLocker pentru dispozitive Windows. Pentru mai multe informații, consultați [setările Windows 10 (și versiunile ulterioare) pentru a proteja dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Ar trebui să știți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker, care este declanșată fără aplicarea politicii MDM. Acest lucru poate afecta aplicarea politicii dacă sunt configurate Setări non-implicite. Consultați următoarele întrebări frecvente pentru mai multe detalii.
 
Pentru informații despre depanarea problemelor cu BitLocker, consultați [Depanarea politicilor BitLocker în Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 Q: ce ediții de criptare dispozitiv de suport Windows utilizând politica de protecție Endpoint?<br>
 A: setările din Intune Endpoint Politica de protecție sunt implementate utilizând CSP-ul [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nu toate edițiile sau compilările de Windows acceptă CSP-ul BitLocker. <br><br>
      În acest moment, sunt acceptate următoarele ediții Windows: Enterprise, Education, mobile, Mobile Enterprise și Professional (compilare 1809 și versiuni ulterioare).
 
Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128), va aplica o politică cu diferite setări declanșează automat re-criptarea unității cu noile setări?<br>
A: nu. Pentru a aplica noile setări de cifrare, unitatea trebuie mai întâi decriptată.<br><br>
**Notă:** Pentru dispozitivele care se înscriu cu autopilot, criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite setările bazate pe politici pentru a fi utilizate în locul implicite de sistem de operare.
 
Î: dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune, va fi decriptat atunci când această politică este eliminată?<br>
A: eliminarea politicii legate de criptare nu duce la decriptarea unităților care au fost configurate.
 
Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are BitLocker activat, chiar dacă este?<br>
A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeaza clientul Windows Device Atestation Health (DHA). Acest client măsoară numai starea dispozitivului la Boot Time. Deci, dacă un dispozitiv nu a fost repornit deoarece criptare BitLocker s-a finalizat, serviciul de client DHA nu va raporta BitLocker ca fiind activ.
 
 