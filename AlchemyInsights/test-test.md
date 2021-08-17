---
title: Termeni care lipsesc din SharePoint de termeni online
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106438"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Activarea Criptării BitLocker cu Intune

Politica de Endpoint Protection Intune poate fi utilizată pentru a configura setările de criptare Boitlocker pentru dispozitive Windows, așa cum este descris în: Setările Windows10 (și mai recente) pentru a proteja dispozitivele care utilizează Intune

Rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată bitlocker care se declanșează fără aplicația politicii MDM. Acest lucru poate afecta aplicația politicii dacă sunt configurate setări neimi setările implicite. Consultați Întrebări frecvente pentru mai multe detalii.


Întrebări frecvente: Ce ediții de Windows acceptă criptarea dispozitivelor utilizând Endpoint Protection politică?
R: Setările din Intune Endpoint Protection sunt implementate utilizând CSP Bitlocker.  Nu toate edițiile și compilări de Windows acceptă CSP Bitlocker. În acest moment, Windows Editions: Enterprise; Sunt acceptate aplicațiile Education, Mobile, Mobile Enterprise și Professional (începând cu versiunea 1809).




Î: Dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite sistem de operare pentru metoda de criptare și puterea de descifrare (XTS-AES-128) va aplica o politică cu setări diferite care declanșează automat re-criptarea unirii cu noile setări?

R: Nu. Pentru a aplica noile setări cipher, unitatea trebuie întâi decriptată.

Notă Pentru dispozitivele înscrise cu AutoPilot, criptarea automată care ar avea loc în timpul OOBE nu este declanșată până când nu se evaluează politica Intune, care permite utilizarea setărilor bazate pe politică în locul valorilor implicite ale OS




Î Dacă un dispozitiv este criptat în urma aplicației politicii Intune, acesta va fi decriptat atunci când este eliminată acea politică?

A: Eliminarea politicii corelate cu criptarea NU are ca rezultat decriptarea unităților care au fost configurate.




Î: De ce politica de conformitate Intune arată că dispozitivul meu nu are "BitLocker Activat", dar este?

A: Setarea "Bitlocker activat" din politica de conformitate Intune utilizează clientul Windows Device Health Attestation (DHA). Acest client măsoară starea dispozitivului doar la momentul de pornire. Așadar, dacă un dispozitiv nu a fost repornit după ce a fost finalizată criptarea bitlocker, serviciul client DHA nu va raporta bitlocker ca fiind activ.