---
title: Blocat în Outbox din cauza atașamente mari
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441317"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Remedierea mesajelor blocate în Outbox

Vă recomandăm să începeți prin rularea scenariului ["am probleme cu trimiterea, primirea sau găsirea mesajelor de e-mail"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistență Microsoft și asistent recuperare](https://diagnostics.office.com/#/) .

Când un mesaj se blochează în Outbox, cele mai probabile cauze sunt:
- Atașamente mari.
- Opțiunea **Trimitere imediată când este conectată** nu este activată.

Pentru a elimina atașamentele mari: 

1. În Outlook, selectați **Trimitere/primire** > **lucru offline**. 
2. În panoul de navigare, selectați **Outbox**. De aici, puteți: 
    - Ștergeți mesajul (selectați-l și apoi selectați **Ștergere**).
    - Glisați mesajul în folderul Schițe, faceți dublu clic pentru a-l deschide și eliminați atașamentul, selectați-l și apoi selectați **Ștergere**).
3. Dacă primiți o eroare care spune că Outlook încearcă să transmită mesajul, închideți Outlook. Este posibil să dureze câteva momente pentru a ieși. Dacă Outlook nu se închide, apăsați Ctrl + Alt + Delete și selectați **Start Task Manager**. În Task Manager, selectați fila **procese** , derulați în jos la Outlook. exe și selectați **Terminare proces**.
4. După ce Outlook se închide, reporniți-l și repetați pașii 2 și 3. 
5. După ce eliminați atașarea, faceți clic pe **Trimitere/primire** > **lucru offline** pentru a relua lucrul online. 

De asemenea, mesajele se blochează în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat. Apasă pe **trimite/primește** și uită-te la butonul de **lucru offline** . Dacă e albastru, ești deconectat. Selectați-l pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere toate**.
 
Pentru a activa **trimiterea imediată când este conectată**:
 
- Selectați **** > **** opțiunile >  de fișier**avansate**.
În secțiunea **Trimitere și primire** , selectați **Trimiteți imediat când sunteți conectat**, apoi alegeți **OK**.
 
Pentru detalii complete, a se vedea:
- [Videoclip: trimiteți sau ștergeți un e-mail blocat](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mail rămâne în folderul Outbox până când inițiați manual o operațiune de trimitere/primire în Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
