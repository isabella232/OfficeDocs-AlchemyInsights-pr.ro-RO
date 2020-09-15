---
title: Monitorizarea accesului condiționat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702915"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorizarea accesului condiționat pentru Exchange

Utilizatorii vizați de Access condițional vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs. Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:
  
- Dacă se presupune că dispozitivul este înscris, consiliați utilizatorul să meargă la aplicația portal a firmei și să verifice dacă apare în portalul firmei. Dacă nu, utilizatorul trebuie să înscrie dispozitivul.
    
- În portalul Azure, accesați ** \> conformitatea dispozitivelor Intune**. Sub **Monitor** , faceți clic pe **conformitate dispozitiv**. Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca fiind conform. 
    
- În portalul Azure, accesați ** \> conformitatea dispozitivelor Intune**. Sub **gestionare**, faceți clic pe **politici**. În lista de politici de conformitate, Verificați dacă un profil este atribuit dispozitivului utilizatorului. Dacă nu este atribuit niciun profil, atunci Intune nu va putea confirma starea de conformitate a dispozitivului. 
    
- Editați atribuirea accesului condiționat al utilizatorului.
    
1. În portalul Azure accesați politicile de ** \> acces condiționale \> Intune**
    
2. Selectați o politică din listă
    
3. Faceți clic pe **utilizatori și grupuri**
    
4. Pentru a viza o anumită politică la o persoană, adăugați-o la lista **Includere** . Pentru a vă asigura că o persoană este omisă din politică, adăugați-o la lista de **excluderi** . 
    
Citiți mai mult: [cum să monitorizați dispozitivele de acces condiționat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

