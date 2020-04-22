---
title: Acces condiționat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706033"
---
# <a name="conditional-access-with-intune"></a>Acces condiționat cu Intune

Utilizarea **accesului condiționat** cu Intune necesită 3 pași: 
  
- Creați o **politică de acces condiționat** care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa aceste resurse. De exemplu, un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul companiei. 
    
- Creați o **politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat compatibil. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat compatibil. 
    
- Asigurarea atât **a politicilor de conformitate,** cât și **a politicilor de acces condiționat** sunt direcționate către grupurile de utilizatori dorite. Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory. 
    
Citește și...
  
- [Cele mai bune practici de acces condiționat](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introducere în Accesul condiționat](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

