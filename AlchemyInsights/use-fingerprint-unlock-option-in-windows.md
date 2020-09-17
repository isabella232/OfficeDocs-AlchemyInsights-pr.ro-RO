---
title: Opțiunea de a utiliza deblocarea amprentelor în Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795256"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Opțiunea de a utiliza deblocarea amprentelor în Windows 10

**Activare amprentă Windows Hello**

Pentru a debloca Windows 10 utilizând amprenta, trebuie să configurați amprenta Windows Hello prin Adăugare (permițând Windows să învețe să recunoască) cel puțin un deget. 

1. Accesați **setări > conturi > opțiuni de conectare** (sau faceți clic [aici](ms-settings:signinoptions?activationSource=GetHelp)). Opțiunile de conectare disponibile vor fi listate. De exemplu:

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. Atingeți sau faceți clic pe **Windows Hello amprentă**, apoi faceți clic pe **configurare**. În fereastra de configurare Windows Hello **, faceți clic pe introducere.** Senzorul de amprentă va fi activat și vi se va solicita să puneți degetul pe senzor:

   ![Senzor de amprentă.](media/fingerprint-sensor.png)

3. Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat degetul. Când se termină acest lucru, veți avea opțiunea de a adăuga alte degete pe care poate doriți să le utilizați pentru conectare. Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a vă folosi amprenta pentru a face acest lucru.

**Amprenta Windows Hello nu este disponibilă ca opțiune de conectare**

Dacă amprenta digitală din Windows Hello nu este afișată ca opțiune în **opțiunile de conectare**, înseamnă că Windows nu este conștient de niciun cititor de amprente/scaner ATAȘAT la PC sau că o politică de sistem îi împiedică utilizarea (dacă, de exemplu, PC-ul este gestionat de locul de muncă). Pentru a depana: 

1. Selectați butonul **Start** în bara de activități și căutați **Manager dispozitive**.

2. Faceți clic sau atingeți pentru a deschide **Manager dispozitive**.

3. În Manager dispozitive, extindeți dispozitivele biometrice făcând clic pe ghilimelele sale.

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. Scanerul de amprente trebuie să fie listat ca dispozitiv biometric, cum ar fi scanerul Synaptics WBDI:

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC-ul dvs., accesați site-ul web al producătorului PC-ului. În secțiunea asistență tehnică pentru modelul PC-ului, căutați un driver Windows 10 pentru un scaner pe care îl puteți instala.

6. Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și a instala software de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.
