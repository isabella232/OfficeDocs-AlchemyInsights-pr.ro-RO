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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241264"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Remedierea mesajelor blocate în Outbox

Vă recomandăm să începeți prin a executa scenariul ["Am probleme cu trimiterea, primirea sau găsirea mesajelor de poștă electronică"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistent de asistență și recuperare Microsoft.](https://diagnostics.office.com/#/)

Atunci când un mesaj devine blocat în Outbox, cauza cea mai probabilă este o atașare mare sau opțiunea "Trimite imediat atunci când este conectat" nu este activată.

**Eliminarea atașării mari**

1. În Outlook, selectați **Trimitere / primire** > **de lucru offline**. 
2. În panoul de navigare, selectați **Outbox**. De aici, puteți: 
    - ºtergeþi mesajul (selectaþi-l ºi apoi **selectaþi ªtergeþi**).
    - Glisați mesajul în folderul Schițe, faceți dublu clic pentru a-l deschide și eliminați atașarea, selectați-l, apoi **selectați Ștergere**).
3. Dacă primiți o eroare care spune Outlook încearcă să transmită mesajul, închideți Outlook. S-ar putea să dureze câteva momente să iasă. Dacă Outlook nu se închide, apăsați Ctrl+Alt+Delete și selectați **Pornire Manager activități**. În Managerul de activități, selectați fila **Procese,** defilați în jos la outlook.exe și selectați **Terminare proces**.
4. După ce Outlook se închide, reporniți-l și repetați pașii 2 și 3. 
5. După ce eliminați atașarea, faceți clic pe **Trimitere / primire** > **lucru offline** pentru a relua lucrul online. 

Mesajele rămân blocate și în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat. Faceți clic pe **Trimitere / Primire** și uitați-vă la butonul Lucru **offline.** Dacă e albastru, ești deconectat. Faceți clic pe ea pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere totală**.
 
**Activare trimitere imediat după conectare**
 
1. Pe fila Fișier, faceți clic pe **Opțiuni**.

2. În caseta de dialog Opțiuni Outlook, faceți clic pe **Complex**.

3. În secțiunea Trimitere și primire, faceți clic pentru a activa **Trimitere imediat când este conectat**. Faceți clic pe **OK**.
 
Pentru detalii complete, consultați:
- [Video: Trimiterea sau ștergerea unui e-mail blocat](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mailrămâne în folderul Outbox până când inițiați manual o operațiune de trimitere / primire în Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
