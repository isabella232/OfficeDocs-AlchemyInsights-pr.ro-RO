---
title: Utilizarea opțiunii de deblocare a amprentelor în Windows 10
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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796689"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utilizarea opțiunii de deblocare a amprentelor în Windows 10

**Activarea amprentelor Windows Hello**

Pentru a debloca Windows 10 folosind amprenta, trebuie să configurați amprentă Windows Hello adăugând (permițând ca Windows să învețe să recunoască) cel puțin un deget. 

1. Accesați Setări **> Conturi > Opțiuni de conectare (sau faceți** clic [aici](ms-settings:signinoptions?activationSource=GetHelp)). Vor fi listate opțiunile disponibile de conectare. De exemplu:

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. Faceți clic sau **atingeți Amprentă Windows Hello**, apoi faceți clic pe **Instalare**. În fereastra de instalare Windows Hello, faceți **clic pe Incepeți.** Senzorul de amprente se va activa și veți fi întrebat dacă puneți degetul pe senzor:

   ![Senzor de amprente.](media/fingerprint-sensor.png)

3. Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat cu degetul. Când se termină aceasta, veți avea opțiunea de a adăuga alte degete pe care poate doriți să le utilizați pentru conectare. Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a utiliza amprenta pentru a face acest lucru.

**Amprentă Windows Hello nu este disponibilă ca opțiune de conectare**

Dacă amprentă Windows Hello nu este afișată ca opțiune de opțiuni de conectare, înseamnă că Windows nu cunoaște niciun cititor de amprente sau scaner atașat la PC sau că o politică de sistem împiedică utilizarea acesteia (de exemplu, **PC-ul** este gestionat de locul de muncă). Pentru a depana: 

1. Selectați **butonul Start** din bara de activități și căutați Manager **dispozitive**.

2. Atingeți sau faceți clic pentru a **deschide Manager dispozitive**.

3. În Manager dispozitive, extindeți Dispozitivele biometrice, făcând clic pe ghilimelele unghiulare.

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. Scanerul de amprente ar trebui să fie listat ca dispozitiv biometric, cum ar fi scanerul de sindicalizare WBDI:

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC, accesați site-ul web al producătorului PC-ului. În secțiunea de asistență tehnică pentru modelul PC, căutați un driver Windows 10 pentru un scaner pe care să îl puteți instala.

6. Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și a instala software-ul de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.
