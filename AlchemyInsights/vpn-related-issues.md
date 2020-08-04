---
title: Probleme legate de VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555229"
---
# <a name="vpn-related-issues"></a>Probleme legate de VPN

Implementarea cu succes a conectivității VPN pentru clienții MDM depinde de un profil implementat care reflectă corect cerințele infrastructurii VPN. Pentru setările corespunzătoare pentru platformele client pe care le investigați, consultați: 

[Setările dispozitivelor holografice Windows 10 și Windows pentru a adăuga conexiuni VPN utilizând Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Adăugarea setărilor VPN pe dispozitivele iOS și iPadOS în Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Setările dispozitivului Android pentru a configura VPN în Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Adăugarea setărilor VPN pe dispozitivele macOS în Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Dacă profilul VPN utilizează autentificarea bazată pe certificat, asigurați-vă că profilurile de certificat de certificat rădăcină și de autentificare client legate la profilul VPN sunt implementate cu succes.

**Probleme comune**

**Am implementat un profil VPN pe un dispozitiv. Intune arată că a avut succes, dar dispozitivul nu se conectează la VPN.**

O stare reușită înseamnă că Intune a implementat cu succes profilul așa a fost configurat. Cu toate acestea, este posibil ca aceste configurații să nu corespundă cerințelor de rețea și/sau autentificare. Examinați jurnalele din serviciul de infrastructură și autentificare (pe serverul VPN și serverul NPS/Radius) pentru mai multe detalii despre a încercat conexiunea. Poate fi necesar să lucrați cu echipa de infrastructură de rețea sau cu furnizorul VPN terț pentru a colecta și a revizui jurnalele.

**Când configurez un VPN personalizat pentru iOS, funcția VPN per aplicație nu este disponibilă.**

VPN per aplicație pentru dispozitivele iOS din Intune este disponibil în prezent pentru o anumită listă de furnizori și parteneri, care trebuie să îndeplinească, de asemenea, cerințele preliminare ale certificatului înainte de a configura un VPN per aplicație. Pentru mai multe informații, consultați [Configurarea rețelei private virtuale (VPN) per aplicație pentru dispozitivele iOS/iPadOS în Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Pentru mai multe informații despre toate tipurile de conexiuni VPN din Intune, consultați [Crearea profilurilor VPN pentru conectarea la serverele VPN din Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN la cerere iOS nu se declanșează atunci când este accesat un domeniu configurat**

Pentru a testa setările VPN automate, setați următoarele valori:

Doresc să fac următoarele: **Evaluați fiecare încercare de conectare** 

Alegeți dacă să vă conectați: **Conectați-vă dacă este necesar**

Când utilizatorii accesează aceste domenii: *nume de domeniu* **țintă**

Dacă configurația de mai sus nu reușește, adăugați următorul element:

Când acest URL este inaccesibil, forțați conectarea VPN: **BADURL**