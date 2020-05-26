---
title: Executarea diagnosticelor de memorie Windows în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357784"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Executarea diagnosticelor de memorie Windows în Windows 10

Dacă Windows și aplicațiile de pe PC se blochează, înghedează sau acționează într-un mod instabil, este posibil să aveți o problemă cu memoria PC-ului (RAM). Aveți posibilitatea să executați Windows Memory Diagnostic pentru a căuta probleme cu memoria RAM a PC-ului.

În caseta de căutare din bara de activități, tastați **diagnosticare memorie**, apoi selectați Diagnosticare **memorie Windows**. 

Pentru a executa diagnosticarea, PC-ul trebuie să repornească. Aveți opțiunea de a reporni imediat (vă rugăm să salvați lucrul și să închideți mai întâi documentele deschise și e-mailurile) sau să programați diagnosticarea să ruleze automat data viitoare când PC-ul repornește:

![Diagnosticare memorie Windows](media/windows-memory-diagnostic.png)

Când PC-ul repornește, **instrumentul de diagnosticare a memoriei Windows** se va executa automat. Starea și progresul vor fi afișate pe măsură ce se execută diagnosticarea și aveți opțiunea de a anula diagnosticarea apăsând tasta **ESC** de pe tastatură.

Când diagnosticarea este finalizată, Windows va porni normal.
Imediat după repornire, când apare Desktopul, va apărea o notificare (lângă pictograma **Centru de acțiune** din bara de activități), pentru a indica dacă s-au găsit erori de memorie. De exemplu:

Iată pictograma Centru de acțiune: ![Pictograma Centru de acțiune](media/action-center-icon.png) 

Și o notificare eșantion: ![Fără erori de memorie](media/no-memory-errors.png)

Dacă ați pierdut notificarea, puteți selecta pictograma **Centru de acțiune** din bara de activități pentru a afișa Centrul de **acțiune** și a vedea o listă de notificări derulantă.

Pentru a revizui informații detaliate, tastați **eveniment** în caseta de căutare din bara de activități, apoi selectați **Vizualizator evenimente**. În panoul din stânga vizualizatorului de **evenimente,** navigați la **Windows Logs > System**. În panoul din dreapta, scanați lista în timp ce căutați coloana **Sursă,** până când vedeți evenimente cu valoare sursă **MemoryDiagnostics-Results**. Evidențiați fiecare astfel de eveniment și vedeți informațiile despre rezultate în caseta de sub fila **General** de sub listă.
