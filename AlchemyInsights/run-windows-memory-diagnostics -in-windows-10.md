---
title: Rulați Windows diagnostice de memorie în Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922583"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Rulați Windows diagnostice de memorie în Windows 10

Dacă Windows și aplicațiile de pe PC se blochează, îngheașează sau acționează într-un mod instabil, este posibil să aveți o problemă cu memoria PC-ului (RAM). Puteți rula programul de Windows de diagnosticare a memoriei pentru a căuta probleme cu memoria RAM a PC-ului.

În caseta de căutare din bara de activități, tastați **diagnostic de** memorie , apoi selectați una Windows **Diagnosticare memorie**. 

Pentru a rula diagnosticarea, PC-ul trebuie să repornească. Aveți opțiunea să reporniți imediat (salvați-vă lucrul și închideți mai întâi documentele și mesajele de e-mail deschise) sau programați diagnosticarea să ruleze automat data următoare când PC-ul repornește:

![Windows Diagnosticare memorie](media/windows-memory-diagnostic.png)

Atunci când PC-ul **repornește, Windows de diagnosticare a memoriei** va rula automat. Starea și progresul se vor afișa pe măsură ce rulează diagnosticele și veți avea opțiunea de a anula diagnosticele apăsând tasta **ESC** pe tastatură.

Când diagnosticarea se termină, Windows începeți normal.
Imediat după repornire, atunci când apare Desktopul,  va apărea o notificare (lângă pictograma Acțiuni din bara de activități), pentru a indica dacă s-au găsit erori de memorie. De exemplu:

Iată pictograma Acțiuni: ![Pictograma Acțiuni](media/action-center-icon.png) 

Și un exemplu de notificare: ![Nicio eroare de memorie](media/no-memory-errors.png)

Dacă nu vedeți notificarea,  puteți selecta pictograma Acțiuni  de pe bara de activități pentru a afișa Acțiuni și a vedea o listă de notificări prin care se poate defila.

Pentru a revizui informațiile detaliate, **tastați eveniment** în caseta de căutare din bara de activități, apoi selectați **Vizualizator evenimente**. În panoul **din stânga** al Vizualizatorului de evenimente, navigați la jurnalele **Windows jurnale > nou.** În panoul din dreapta, scanați lista în timp ce priviți coloana **Sursă,** până când vedeți evenimente cu valoarea sursă **MemoryDiagnostics-Results.** Evidențiați fiecare astfel de eveniment și vedeți informațiile despre rezultate în caseta de **sub fila General** de sub listă.
