---
title: Setările de pornire în Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751147"
---
# <a name="startup-settings-in-windows-10"></a>Setările de pornire în Windows 10

**Modificarea aplicațiilor care rulează automat la pornire**

1. Accesați [setări > aplicații > pornire](ms-settings:startupapps?activationSource=GetHelp).

2. Asigurați-vă că orice aplicație **pe**care doriți să o difuzați la pornire este activată.

**Adăugarea unei aplicații pentru rulare automată la pornire**

1. Atingeți sau faceți clic pe **Start** și găsiți aplicația pe care doriți să o difuzați la pornire.

2. Faceți clic dreapta pe aplicație, faceți clic pe **mai multe**, apoi faceți clic pe **Deschidere locație fișier**. Aceasta deschide locația în care se salvează comanda rapidă către aplicație. Dacă nu există nicio opțiune pentru locația de fișier deschisă, înseamnă că aplicația nu poate fi executată la pornire.

3. Cu locația de fișier deschisă, apăsați **tasta siglă Windows + R**, tastați **Shell: Startup**, apoi faceți clic pe **OK**. Astfel se deschide folderul Startup.

4. Copiați și lipiți comanda rapidă către aplicație din locația fișierului în folderul Startup.

**Opțiuni complexe de pornire (inclusiv modul de siguranță, setările UEFI și pornirea de pe un alt dispozitiv)**

1. Salvați-vă lucrul și închideți toate documentele deschise, deoarece acești pași vor reporni PC-ul.

2. Accesați [setări > actualizare & securitate > recuperare](ms-settings:recovery?activationSource=GetHelp).

3. Sub **pornire complexă**, faceți clic pe **Repornire acum**. 

4. După ce PC-ul repornește la ecranul Alegeți o opțiune:

    - Pentru a porni de pe un dispozitiv, cum ar fi o unitate USB, faceți clic pe **utilizare dispozitiv**.

    - Pentru a introduce setările UEFI (numite uneori configurare BIOS), faceți clic pe **Depanarea > opțiuni complexe > setările de firmware UEFI**. 

    - Pentru a intra în modul de siguranță sau pentru a modifica setările de pornire complexe, faceți clic pe **depanare > opțiuni complexe > setări de pornire**, apoi faceți clic pe **Repornire**. Este posibil să vi se solicite să introduceți [cheia de recuperare BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). După repornirea PC-ului, faceți clic pe setarea de pornire pe care doriți să o utilizați.