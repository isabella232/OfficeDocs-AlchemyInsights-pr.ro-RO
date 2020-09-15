---
title: Depanarea monitorului existent
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690723"
---
# <a name="troubleshoot-an-existing-monitor"></a>Depanarea unui monitor existent

Încercați aceste soluții pentru a depana un monitor. 

**Reîmprospătați ecranul monitorului:**

Apăsați simultan tastele următoare: tasta Windows + Ctrl + Shift + B. Aceasta va reîmprospăta comunicarea cu driverul grafic. Monitoarele dumneavoastră vor clipi imediat și revin după câteva secunde.

**Depanarea hardware-ului monitorului:**

1. Deconectați cablul la conectarea PC-ului la monitor și conectați-l din nou.
2. Deconectați toate dispozitivele neesențiale de pe PC (cum ar fi adaptoare sau docuri).

**Dacă ați instalat recent o actualizare pe PC, puteți să reveniți la driverul de afișare:**

1. Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.
2. Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare, selectați **Proprietăți**.
3. Navigați la fila **driver** și selectați **driver roll back**. <br>
Notă: dacă acest lucru nu este disponibil sau este estompat, selectați **nu** din opțiunile de mai jos pentru a trece la pasul următor.
4. Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.

**Dezinstalați și reinstalați driverul de afișare:**

1. Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.
2. Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare, selectați **Dezinstalare dispozitiv**. 
3. Bifați caseta de lângă **Ștergeți software-ul de driver pentru acest dispozitiv** și selectați **Dezinstalare**.<br>
Notă: este posibil să vi se solicite să reporniți computerul în acest moment. Asigurați-vă că scrieți instrucțiunile rămase înainte de a reporni.
4. Deschideți din nou Device Manager.
5. Extindeți secțiunea **adaptoare de afișare** , faceți clic cu butonul din dreapta pe adaptorul de afișare și selectați **actualizați driverul**.
6. Selectați **Căutare automată pentru actualizare software de driver** și urmați instrucțiunile de instalare.