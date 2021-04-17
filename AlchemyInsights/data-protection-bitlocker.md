---
title: Protecția datelor - BitLocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815627"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea criptării BitLocker cu Intune

Politica de protecție pentru punctul final Intune poate fi utilizată pentru a configura setările de criptare Bitlocker pentru dispozitive Windows. Pentru mai multe informații, consultați [Setările Windows 10 (și mai recente) pentru a proteja dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

În plus față de Politica de protecție pentru punctele finale, există și un raport de criptare care furnizează o vizualizare mai detaliată a stării de criptare pentru dispozitive. Acest raport poate fi accesat din portalul MEM de sub **Dispozitive > Monitor,** apoi, sub Configurație, **selectați** [Raport de criptare.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Dacă descoperiți că BitLocker nu poate fi activat așa cum vă așteptați sau că profilul utilizat pentru a activa BitLocker se află într-o stare de eroare, revizuiți raportul de criptare pentru a înțelege mai bine de ce apare comportamentul.

Pentru a găsi detalii despre cum să interpretați raportul, inclusiv diversele valori de stare a criptării, consultați [Monitorizarea criptării dispozitivelor cu Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea bitlocker automată, care este declanșată fără aplicația politicii MDM. Acest lucru poate afecta aplicația politicii dacă sunt configurate setări neimi setările implicite. Consultați următoarele Întrebări frecvente pentru mai multe detalii.

Pentru informații despre depanarea problemelor cu bitLocker, consultați [Depanarea politicilor BitLocker în Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**ÎNTREBĂRI FRECVENTE**

Î: Ce ediții de Windows acceptă criptarea dispozitivelor utilizând Politica de protecție a punctului final?<br>
R: Setările din Politica de protecție pentru punctul final Intune sunt implementate utilizând [CSP Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nu toate edițiile sau compilări de Windows acceptă CSP Bitlocker. <br><br>

Î: Cum poate fi activat BitLocker pe dispozitive fără să fie necesară interacțiunea utilizatorului final?<br>
A: Atât timp cât sunt îndeplinite cerințele prealabile necesare, este posibil să activați Bitlocker "Criptarea silențioasă" prin Intune. Consultați detaliile despre cerințele dispozitivului și, de exemplu, setările de politică pentru a activa criptarea silențioasă în următorul document: [Activarea silențioasă a criptării BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

Î: Dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite sistem de operare pentru metoda de criptare și puterea de descifrare (XTS-AES-128), va aplica o politică cu setări diferite care declanșează automat re-criptarea unii cu noile setări?<br>
R: Nu. Pentru a aplica noile setări cipher, unitatea trebuie mai întâi decriptată.<br><br>
**Notă:** Pentru dispozitivele înscrise cu AutoPilot, criptarea automată care ar avea loc în timpul OOBE nu este declanșată până când nu se evaluează politica Intune, care permite utilizarea setărilor bazate pe politică în locul valorilor implicite ale OS.
 
Î: Dacă un dispozitiv este criptat ca rezultat al aplicației politicii Intune, va fi decriptat atunci când acea politică este eliminată?<br>
A: Eliminarea politicii legate de criptare NU are ca rezultat decriptarea unităților care au fost configurate.
 
Î: De ce Politica de conformitate Intune arată că dispozitivul meu nu are BitLocker activat, chiar dacă este activat?<br>
A: Setarea "Bitlocker activat" din Politica de conformitate Intune utilizează clientul Windows Device Health Attestation (DHA). Acest client măsoară starea dispozitivului doar la momentul de pornire. Așadar, dacă un dispozitiv nu a fost repornit de când a fost finalizată criptarea Bitlocker, serviciul client DHA nu va raporta Bitlocker ca fiind activ.
 
 