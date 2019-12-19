---
title: Depanarea monitorului existent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738580"
---
# <a name="troubleshoot-an-existing-monitor"></a>Depanarea unui monitor existent

Încercați aceste soluții pentru a depana un monitor. 

**Reîmprospătați ecranul monitorului:**

Apăsați următoarele taste în același timp: Windows key + Ctrl + Shift + B. Acest lucru va reîmprospăta comunicarea cu driverul grafic. Monitoarele tale vor clipi momentan și se întorc după câteva secunde.

**Depanarea monitorului hardware:**

1. Deconectați cablul care conectează PC-ul la monitor și conectați-l la loc.
2. Deconectați orice dispozitive neesențiale de pe PC (cum ar fi adaptoare sau docuri).

**Dacă ați instalat recent o actualizare pe PC, aveți posibilitatea să reveniți la driverul de afișare:**

1. Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.
2. Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare, ANDS selectați **Proprietăți**.
3. Navigați la fila **driver** și selectați **Roll Back Driver**. <br>
Notă: dacă acest lucru nu este disponibil sau este gri, selectați **nu** din opțiunile de mai jos pentru a trece la pasul următor.
4. Poate fi necesar să reporniți PC-ul înainte ca aceste modificări să aibă efect.

**Dezinstalați și reinstalați driverul de afișare:**

1. Selectați **Start**, tastați **Manager dispozitive**și selectați **Manager dispozitive** din rezultate.
2. Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare, ANDS selectați **Dezinstalare dispozitiv**. 
3. Bifați caseta de lângă **ștergerea software-ului de driver pentru acest dispozitiv** și selectați **Dezinstalare**.<br>
Notă: este posibil să fiți rugat să reporniți computerul în acest stadiu. Asigurați-vă că notați instrucțiunile rămase înainte de a reporni.
4. Deschideți din nou managerul de dispozitive.
5. Extindeți secțiunea **adaptoare de afișare** , faceți clic dreapta pe adaptorul de afișare și selectați **Actualizare driver**.
6. Selectați **Căutare automată pentru software-ul de driver de actualizare** și urmați instrucțiunile de instalare.