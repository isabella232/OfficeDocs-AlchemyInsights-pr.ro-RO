---
title: Problemă cu filtrul atribut și definire
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482919"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problemă cu filtrul atribut și definire

**Problemă cu valorile UPN conflictuale**

Ziua de lucru pentru ca utilizatorul de publicitate să aibă acces la ziua de lucru pentru asigurarea accesului utilizatorilor de reclame afișează mesajul de eroare **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Operațiunea nu a reușit, deoarece valoarea UPN furnizată pentru Adăugare/modificare nu este unică la nivel de pădure. Detalii despre eroare: **CONSTRAINT_ATT_TYPE-UserPrincipalName**.

Valoarea **UserPrincipalName** pe care un conector de zi de lucru încearcă să o seteze atunci când creați contul de utilizator al reclamei există deja în domeniul de anunțuri țintă. Acest lucru implică faptul că, fie (1) utilizatorul există deja, iar verificarea ID-ului de potrivire nu a reușit pentru utilizator sau (2) regula de generare a UPN a generat o valoare conflictuală.

Iată pașii de rezolvare sugerați:

Dacă utilizatorul există deja și verificarea ID-ului care se potrivește nu a reușit să conecteze contul zile lucrătoare la contul Active Directory, Verificați dacă atributul ID corespondent (de obicei **IDAngajat**) atât în ziua de lucru, cât și în anunț au o potrivire exactă. Dacă nu au o corespondență, este o problemă de date care trebuie remediată. De exemplu, dacă IDAngajat din ziua lucrătoare este 001052 și în AD este 1052, atunci motorul de asigurare a accesului nu va reuși să conecteze cele două conturi și va încerca să creeze un utilizator care există deja. Soluția în acest caz este să modificați valoarea **IDAngajat** din AD pentru a include zerouri inițiale pentru a-l face 001052.
Dacă expresia generatoare de UPN nu generează o valoare unică, luați în considerare utilizarea funcției de duplicare **SelectUniqueValue** pentru a genera o valoare unică de fiecare dată.

**Ziua de lucru pentru asigurarea accesului utilizatorilor AD nu setează valoarea atributului Manager pentru contul de utilizator al RECLAMEi**

Lucrarea de lucru de ziua de lucru pentru asigurarea accesului utilizatorilor AD nu stabilește valoarea de atribut **Manager** pentru conturile de utilizator de publicitate. Există două scenarii posibile atunci când se vede acest comportament:

1. Managerul din ziua de lucru nu poate fi rezolvat într-un cont de utilizator de publicitate corespunzător, deoarece managerul nu este în domeniul de aplicare.
2. Într-un scenariu **mai multe domenii de publicitate** , managerul din ziua de lucru nu este prezent în același domeniu cu utilizatorul.

Încercați acești pași pentru a rezolva problema:

1. Dacă ați definit filtrele de definire, verificați mai întâi dacă managerul este în domeniu și îndeplinește clauza de definire. În cazul în care managerul nu îndeplinește filtrul de definire, modificați filtrul, astfel încât managerul să fie, de asemenea, în domeniul operațiunii de asigurare a accesului.
2. Dacă aveți mai multe domenii de publicitate, conectorul are o limitare cunoscută a incapacității de a rezolva referințele managerului de domenii.

Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea accesului automat, consultați [Tutorial: Configurarea zilei de lucru pentru asigurarea accesului automat la utilizatori](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













