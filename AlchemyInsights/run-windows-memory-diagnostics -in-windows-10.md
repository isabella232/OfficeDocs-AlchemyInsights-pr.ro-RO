---
title: Rulați Diagnostice memorie Windows în Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826679"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Rulați Diagnostice memorie Windows în Windows 10

Dacă Windows și aplicațiile de pe PC se blochează, îngheașează sau acționează într-un mod instabil, este posibil să aveți o problemă cu memoria PC-ului (RAM). Puteți rula Diagnostic memorie Windows pentru a căuta probleme cu RAM-ul PC-ului.

În caseta de căutare din bara de activități, tastați **diagnostic de memorie**, apoi selectați Diagnosticare memorie **Windows**. 

Pentru a rula diagnosticarea, PC-ul trebuie să repornească. Aveți opțiunea să reporniți imediat (salvați-vă lucrul și închideți mai întâi documentele și mesajele de e-mail deschise) sau programați diagnosticarea să ruleze automat data următoare când PC-ul repornește:

![Diagnosticare memorie Windows](media/windows-memory-diagnostic.png)

Atunci când PC-ul repornește, **Instrumentul de diagnosticare a memoriei Windows** va rula automat. Starea și progresul se vor afișa pe măsură ce rulează diagnosticele și veți avea opțiunea de a anula diagnosticele apăsând tasta **ESC** pe tastatură.

Atunci când diagnosticele sunt finalizate, Windows va porni normal.
Imediat după repornire, atunci când apare Desktopul,  va apărea o notificare (lângă pictograma Acțiuni din bara de activități), pentru a indica dacă s-au găsit erori de memorie. De exemplu:

Iată pictograma Acțiuni: ![Pictograma Acțiuni](media/action-center-icon.png) 

Și un exemplu de notificare: ![Nicio eroare de memorie](media/no-memory-errors.png)

Dacă nu vedeți notificarea,  puteți selecta pictograma Acțiuni  de pe bara de activități pentru a afișa Acțiuni și a vedea o listă de notificări prin care se poate defila.

Pentru a revizui informațiile detaliate, **tastați eveniment** în caseta de căutare din bara de activități, apoi selectați **Vizualizator evenimente**. În panoul **din stânga** al Vizualizatorului de evenimente, navigați la **Jurnale Windows > Sistem**. În panoul din dreapta, scanați lista în timp ce priviți coloana **Sursă,** până când vedeți evenimente cu valoarea sursă **MemoryDiagnostics-Results.** Evidențiați fiecare astfel de eveniment și vedeți informațiile despre rezultate în caseta de **sub fila General** de sub listă.
