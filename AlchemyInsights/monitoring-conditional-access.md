---
title: Monitorizarea accesului condiționat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713730"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorizarea accesului condiționat pentru exchange

Utilizatorii vizați cu acces condiționat vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs. Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:
  
- Dacă se presupune că dispozitivul este înscris, sfătuiți utilizatorul să meargă la aplicația Portal companie și verificați dacă apare în portalul companiei. Dacă nu, utilizatorul ar trebui să înscrie dispozitivul.
    
- În portalul Azure accesați **Intune \> dispozitiv conformitate**. Sub **Monitor,** faceți clic pe **Conformitate dispozitiv**. Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca compatibil. 
    
- În portalul Azure accesați **Intune \> dispozitiv conformitate**. Sub **Gestionare**, faceți clic pe **Politici**. În lista de politici de conformitate, verificați dacă un profil este atribuit dispozitivului utilizatorului. Dacă nu este atribuit niciun profil, Intune nu va putea confirma starea de conformitate a dispozitivului. 
    
- Editați atribuirea de acces condiționat a utilizatorului.
    
1. În portalul Azure accesați ** \> Intune \> condițională accesați politicile de acces**
    
2. Selectarea unei politici din listă
    
3. Faceți clic pe **Utilizatori și grupuri**
    
4. Pentru a viza o anumită politică către o persoană, adăugați-le în lista **Includere.** Pentru a vă asigura că o persoană este omisă din politică, adăugați-le la lista **Excludere.** 
    
Citiți mai mult: [Cum se monitorizează dispozitivele de acces condiționat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

