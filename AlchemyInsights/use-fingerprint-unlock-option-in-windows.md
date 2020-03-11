---
title: Utilizarea opțiunii de deblocare a amprentelor digitale în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588327"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utilizarea opțiunii de deblocare a amprentelor digitale în Windows 10

**Activare amprentă windows hello**

Pentru a debloca Windows 10 utilizând amprenta, trebuie să configurați Windows Hello Fingerprint adăugând (lăsând Windows să învețe să recunoască) cel puțin un deget. 

1. Accesați **Setări > conturi > opțiuni de conectare** (sau faceți clic [aici](ms-settings:signinoptions?activationSource=GetHelp)). Vor fi listate opțiunile de conectare disponibile. De exemplu:

    ![Opțiuni de conectare.](media/sign-in-options.png)

2. Faceți clic sau atingeți **Windows Hello Fingerprint**, apoi faceți clic pe **Configurare**. În fereastra de configurare Windows Hello, faceți clic pe **Introducere**. Senzorul de amprentă se va activa și vi se va cere să plasați degetul pe senzor:

   ![Senzor de amprentă.](media/fingerprint-sensor.png)

3. Urmați instrucțiunile, care vă vor solicita să scanați în mod repetat degetul. Când se termină acest lucru, veți avea opțiunea de a adăuga alte degete pe care doriți să le utilizați pentru conectare. Data viitoare când vă conectați la Windows 10, veți avea opțiunea de a utiliza amprenta pentru a face acest lucru.

**Windows Hello Fingerprint nu este disponibil ca opțiune de conectare**

Dacă Windows Hello Fingerprint nu este afișat ca opțiune în **opțiunile**de conectare , înseamnă că Windows nu are cunoștință de niciun cititor/scaner de amprente atașat la PC sau că o politică de sistem împiedică utilizarea acestuia (dacă, de exemplu, PC-ul este gestionat de locul de muncă). Pentru a depana: 

1. Selectați butonul **Start** din bara de activități și căutați **Manager dispozitive**.

2. Faceți clic sau atingeți pentru a deschide **Manager dispozitive**.

3. În Manager dispozitive, extindeți Dispozitive biometrice făcând clic pe simbolul său.

   ![Dispozitive biometrice.](media/biometric-devices.png)

4. Scanerul de amprente trebuie listat ca dispozitiv biometric, ar fi scanerul Synaptics WBDI:

   ![Dispozitive biometrice.](media/biometric-devices-expanded.png)

5. Dacă scanerul de amprente nu este afișat și scanerul este integrat în PC, accesați site-ul web al producătorului PC-ului. În secțiunea asistență tehnică pentru modelul PC-ului dvs., căutați un driver Windows 10 pentru un scaner pe care îl puteți instala.

6. Dacă scanerul este separat de PC (atașat prin USB), accesați site-ul web al producătorului scanerului pentru a găsi și instala software-ul de driver de dispozitiv Windows 10 pentru modelul de scaner pe care îl aveți.
