---
title: Blocat în Outbox din cauza atașărilor mari
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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232642"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Remedierea mesajelor blocate în Outbox

Vă recomandăm să începeți prin a executa scenariul ["Am probleme cu trimiterea, primirea sau găsirea mesajelor de poștă electronică"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistent de asistență și recuperare Microsoft](https://diagnostics.office.com/#/) de pe computerul afectat.

Atunci când un mesaj devine blocat în Outbox, cauza cea mai probabilă este o atașare mare sau opțiunea "Trimite imediat atunci când este conectat" nu este activată.

**Eliminarea atașării mari**

1. Faceți clic pe **Trimitere/ Primire** > **lucru offline**. 
2. În panoul de navigare, faceți clic pe **Outbox**. De aici, puteți: 
    - Ștergeți mesajul. Trebuie doar să-l selectați și faceți clic pe **Ștergere**.
    - Glisați mesajul în **folderul schițe ,** faceți dublu clic pentru a deschide mesajul și ștergeți atașarea (faceți clic pe el și faceți clic pe **Ștergere**).
3. Dacă o eroare vă spune că Outlook încearcă să transmită mesajul, închideți Outlook. S-ar putea să dureze câteva momente să iasă. Dacă Outlook nu se închide, **apăsați Ctrl+Alt+Delete** și faceți clic pe **Pornire Manager de activități**. În Managerul de activități, selectați fila **Procese,** defilați în jos la outlook.exe și faceți clic pe **Terminare proces**.
4. După ce Outlook se închide, reporniți Outlook și repetați pașii 2-3. 
5. După ce eliminați atașarea, faceți clic pe **Trimitere / primire** > **de lucru offline** pentru a deselecta butonul și pentru a relua lucrul online. 

Mesajele rămân blocate și în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat. Faceți clic pe **Trimitere / Primire** și uitați-vă la butonul Lucru **offline.** Dacă e albastru, ești deconectat. Faceți clic pe ea pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere totală**.
 
**Activare trimitere imediat după conectare**
 
1. Pe fila Fișier, faceți clic pe **Opțiuni**.

2. În caseta de dialog Opțiuni Outlook, faceți clic pe **Complex**.

3. În secțiunea Trimitere și primire, faceți clic pentru a activa **Trimitere imediat când este conectat**. Faceți clic pe **OK**.
 
Pentru detalii complete, consultați:
- [Video: Trimiterea sau ștergerea unui e-mail blocat](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mailrămâne în folderul Outbox până când inițiați manual o operațiune de trimitere / primire în Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
