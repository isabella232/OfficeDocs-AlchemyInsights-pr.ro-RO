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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037946"
---
# <a name="free-up-drive-space-in-windows-10"></a>Eliberați spațiu pe disc în Windows 10

Iată două opțiuni pentru a elibera spațiu pe hard disk în Windows:

- Eliberați spațiu pe disc în Windows 10.
- Eliberați spațiu pentru actualizările Windows 10 cu dispozitivul de stocare extern.

Dacă încă aveți spațiu-disc redus după ce utilizați Curățare disc, este posibil ca folderul temp să se completeze rapid cu fișiere de aplicație (. imbinare) utilizate de Microsoft Store. Pentru a remedia această problemă, resetați magazinul, debifați memoria cache a magazinului, apoi rulează depanatorul Windows Update. Asigurați-vă că Microsoft Store este închis înainte de a continua cu acești pași.

**Pasul 1: reinițializați Magazinul Microsoft**

**Notă** Acest lucru șterge definitiv datele aplicației pe dispozitiv, inclusiv preferințele și detaliile de conectare.

1. Selectați   >  **Setări** pornire aplicații  >  **aplicații**  >  **& caracteristici**.

1. În lista de aplicații, găsiți și selectați Microsoft Store.

1. Selectați **Opțiuni complexe**.

1. Defilați în jos și selectați **Reinițializare**, apoi **confirmați resetare**.

**Pasul 2: debifați memoria cache a magazinului Microsoft**

1. Apăsați tasta siglă Windows + R pentru a deschide caseta de dialog rulare.

1. Tastați wsreset.exe și selectați **OK**.

1. Se deschide o fereastră de linie de comandă necompletată. După aproximativ 10 secunde, se închide fereastra, iar magazinul se deschide automat.

**Pasul 3: Resetarea Windows Update**

1. Selectați   >  Actualizare **Setări** pornire  >  **& depanare de securitate**  >  .

1. Defilați în jos și selectați **Windows Update** din listă și selectați **rulare depanatorul**.

1. Reporniți computerul și verificați dacă încă întâmpinați problema.

