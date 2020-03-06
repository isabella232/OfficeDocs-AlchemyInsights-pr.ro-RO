---
title: Setările de pornire în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409233"
---
# <a name="startup-settings-in-windows-10"></a>Setările de pornire în Windows 10

**Modificarea aplicațiilor care se execută automat la pornire**

1. Accesați [Setări > aplicații > pornire](ms-settings:startupapps?activationSource=GetHelp).

2. Asigurați-vă că orice aplicație pe care doriți să o rulați la pornire este **activată**.

**Adăugarea unei aplicații pentru a rula automat la pornire**

1. Faceți clic sau **atingeți Start** și găsiți aplicația pe care doriți să o rulați la pornire.

2. Faceți clic cu butonul din dreapta pe aplicație, faceți clic pe **Mai multe**, apoi faceți clic pe Deschidere **locație fișier**. Aceasta deschide locația în care este salvată comanda rapidă către aplicație. Dacă nu există nicio opțiune pentru locația fișierului Deschis, înseamnă că aplicația nu se poate executa la pornire.

3. Cu locația fișierului deschisă, apăsați **tasta siglă Windows + R**, tastați **shell:startup**, apoi faceți clic pe **OK**. Aceasta deschide folderul Startup.

4. Copiați și lipiți comanda rapidă către aplicație din locația fișierului în folderul Startup.

**Opțiuni avansate de pornire (inclusiv Safe Mode, setări UEFI și pornire de pe alt dispozitiv)**

1. Salvați lucrul și închideți toate documentele deschise, deoarece acești pași vor reporni PC-ul.

2. Accesați [Setări > Actualizați & recuperare > securitate](ms-settings:recovery?activationSource=GetHelp).

3. Sub **Pornire complexă**, faceți clic pe **Repornire acum**. 

4. După ce PC-ul repornește la ecranul Alegeți o opțiune:

    - Pentru a porni de pe un dispozitiv, ar fi o unitate USB, faceți clic pe **Utilizare dispozitiv**.

    - Pentru a introduce setările UEFI (denumite uneori configurare BIOS), faceți clic pe **Depanare > Opțiuni complexe > Setări firmware UEFI**. 

    - Pentru a intra în Modul de siguranță sau pentru a modifica setările complexe de pornire, faceți clic pe **Depanare > Opțiuni complexe > Setări pornire**, apoi faceți clic pe **Repornire**. Este posibil să vi se solicite să introduceți cheia de [recuperare BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). După ce PC-ul repornește din nou, faceți clic pe setarea de pornire pe care doriți să o utilizați.