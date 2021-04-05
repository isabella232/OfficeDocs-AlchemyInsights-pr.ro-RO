---
title: Eliberați spațiu pe disc în Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505368"
---
# <a name="free-up-drive-space-in-windows-10"></a>Eliberați spațiu pe disc în Windows 10

Iată două opțiuni pentru a elibera spațiu pe disc în Windows:

- Eliberați spațiu pe disc în Windows 10.
- Eliberați spațiu pentru actualizările Windows 10 cu dispozitivul de stocare extern.

Dacă aveți în continuare spațiu pe disc redus după ce utilizați Curățare disc, este posibil ca folderul Temp să se umple rapid cu fișiere de aplicație (.appx) utilizate de Magazinul Microsoft. Pentru a remedia această problemă, resetați Magazinul, goliți memoria cache a Magazinului, apoi rulați depanatorul Windows Update. Asigurați-vă că Magazinul Microsoft este închis înainte să continuați cu acești pași.

**Pasul 1: Resetați Magazinul Microsoft**

**Rețineți** Acest lucru șterge definitiv datele de aplicație de pe dispozitiv, inclusiv preferințele dvs. și detaliile de conectare.

1. Selectați **Pornire** > **Setări** > **Aplicații** > **Aplicații și caracteristici**.

1. În lista de aplicații, găsiți și selectați Magazinul Microsoft.

1. Selectați **Opțiuni complexe**.

1. Defilați în jos și selectați **Resetare**, apoi faceți clic **Confirmare resetare**.

**Pasul 2: Goliți memoria cache a Magazinului Microsoft**

1. Apăsați tasta siglă Windows + R pentru a deschide caseta de dialog Executare.

1. Tastați wsreset.exe și selectați **OK**.

1. Se deschide o fereastră Linie de comandă goală. După aproximativ 10 secunde, fereastra se închide și Magazinul se deschide automat.

**Pasul 3: Resetați Windows Update**

1. Selectați **Pornire** > **Setări** > **Actualizare și securitate** > **Depanare**.

1. Defilați în jos și selectați **Windows Update** din listă, apoi selectați **Rulați depanatorul**.

1. Reporniți-vă computerul și verificați dacă încă vă confruntați cu această problemă.

