---
title: Monitorizare acces condiționat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307742"
---
# <a name="monitoring-conditional-access"></a>Monitorizare acces condiționat

Utilizatorii orientate cu acces condiționat vor primi un e-mail de notificare, în cazul în care nu îndeplinesc cerinţele de acces al organizaţiei. Pentru a rezolva, va recomandam unul sau mai multe dintre următoarele soluții:
  
- În cazul în care dispozitivul este prezumată a fi înscrişi, sfătui utilizatorul să accesaţi aplicaţia Portal de companie şi să verifice că acesta apare în portalul companiei. Dacă nu, utilizatorul ar trebui să înscrieţi-vă dispozitivul.
    
- În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**. Sub **monitorul de** faceţi clic pe **dispozitiv conformitatea**. Vezi dispozitiv conformitatea raport pentru a verifica că utilizatorul final este marcat ca conforme. 
    
- În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**. La **administrare**, faceţi clic pe **politici**. În lista de conformitatea politicilor, verificaţi că un profil este atribuit de utilizator pe dispozitiv. Dacă este alocat nici un profil, apoi Intune nu va fi capabil să confirme statutul de conformitatea dispozitivului. 
    
- Editare cesiune de acces condiționat utilizatorului.
    
1. În portalul azuriu Du-te la **Intune \> acces condiţionat \> politici**
    
2. Selectaţi o politică din lista
    
3. Faceţi clic pe **utilizatori și grupuri**
    
4. Pentru a-ţintă o anumită politică la cineva, adăugaţi-le la lista de **includeri** . Pentru a se asigura că o persoană este omis din politica, adăugaţi-le la lista de **Exclude** . 
    
Citeşte mai departe: [modul de acces condiționat Monitor dispozitive](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

