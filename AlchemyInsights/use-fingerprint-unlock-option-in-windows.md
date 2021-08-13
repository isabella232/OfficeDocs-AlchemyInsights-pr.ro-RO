---
title: Utilizați opțiunea de deblocare a amprentelor Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971947"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utilizați opțiunea de deblocare a amprentelor Windows 10

**Activarea Windows Hello amprentă digitală**

Pentru a Windows 10 amprentele utilizându-vă amprenta, trebuie să configurați o amprentă Windows Hello adăugând (permițându-i Windows să învețe să recunoască) cel puțin un deget. 

1. Accesați Conturi **Setări > din > de conectare (sau faceți** clic [aici).](ms-settings:signinoptions?activationSource=GetHelp) Vor fi listate opțiunile disponibile de conectare. De exemplu:

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. Atingeți sau faceți **clic Windows Hello amprentă** digitală , apoi faceți clic pe **Configurarea**. În fereastra de Windows Hello inițializare, faceți **clic pe Incepeți.** Senzorul de amprente se va activa și veți fi întrebat dacă puneți degetul pe senzor:

   ![Senzor de amprente.](media/fingerprint-sensor.png)

3. Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat cu degetul. Când se termină aceasta, veți avea opțiunea de a adăuga alte degete pe care poate doriți să le utilizați pentru conectare. Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a utiliza amprenta pentru a face acest lucru.

**Windows Hello Amprentă indisponibilă ca opțiune de conectare**

Dacă Windows Hello amprentă nu este afișată ca opțiune de opțiuni de conectare, înseamnă că Windows nu cunoaște niciun cititor de amprente sau scaner atașat la PC sau că politica de sistem împiedică utilizarea acesteia (dacă, de exemplu, **PC-ul** este gestionat de locul de muncă). Pentru a depana: 

1. Selectați **butonul Start** din bara de activități și căutați Manager **dispozitive**.

2. Atingeți sau faceți clic pentru a **deschide Manager dispozitive**.

3. În Manager dispozitive, extindeți Dispozitivele biometrice, făcând clic pe ghilimelele unghiulare.

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. Scanerul de amprente ar trebui să fie listat ca dispozitiv biometric, cum ar fi scanerul de sindicalizare WBDI:

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC, accesați site-ul web al producătorului PC-ului. În secțiunea de asistență tehnică pentru modelul dvs. de PC, căutați un driver Windows 10 pentru un scaner pe care să îl puteți instala.

6. Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru Windows 10 găsi și instala software-ul de driver de dispozitiv pentru modelul de scaner pe care îl aveți.
