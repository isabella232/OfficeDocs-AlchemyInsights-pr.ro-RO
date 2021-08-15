---
title: Depanarea monitorului existent
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
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981089"
---
# <a name="troubleshoot-an-existing-monitor"></a>Depanarea unui monitor existent

Încercați aceste soluții pentru a depana un monitor. 

**Reîmprospătarea ecranului monitorului:**

Apăsați în același timp următoarele taste: Windows + Ctrl + Shift + B. Astfel, se va reîmprospăta comunicarea cu driverul grafic. Monitoarele dvs. vor clipi imediat și vor reveni după câteva secunde.

**Depanarea componentelor hardware ale monitorului:**

1. Deconectați cablul care conectează PC-ul la monitor și conectați-l din nou.
2. Deconectați toate dispozitivele nee esențiale de la PC (cum ar fi adaptoare sau andocare).

**Dacă ați instalat recent o actualizare pe PC, puteți să reveniți la driverul de afișare:**

1. Selectați **Start**, **tastați manager dispozitive** și **selectați Manager** dispozitive din rezultate.
2. Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Proprietăți**.
3. Navigați la fila **Driver** și selectați **Revenire driver**. <br>
Notă: Dacă nu este disponibilă sau este estompată, selectați **Nu** din opțiunile de mai jos pentru a trece la pasul următor.
4. Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.

**Dezinstalați și reinstalați driverul de afișare:**

1. Selectați **Start**, **tastați manager dispozitive** și **selectați Manager** dispozitive din rezultate.
2. Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Dezinstalare dispozitiv**. 
3. Bifați caseta de lângă Ștergeți **software-ul de driver pentru acest dispozitiv și** selectați **Dezinstalare**.<br>
Notă: Este posibil să i se solicită să reporniți computerul în această etapă. Asigurați-vă că scrieți instrucțiunile rămase înainte de a reporni.
4. Deschideți din nou Manager dispozitive.
5. Extindeți **secțiunea Plăci video,** faceți clic dreapta pe adaptorul de afișare și selectați **Actualizare driver**.
6. Selectați **Căutați automat software de actualizare a driverului** și urmați instrucțiunile de instalare.