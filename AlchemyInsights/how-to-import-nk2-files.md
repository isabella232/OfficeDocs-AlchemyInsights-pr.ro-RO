---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043218"
---
# <a name="how-to-import-nk2-files"></a>Cum se importă fișierele .nk2 

Atunci când porniți Microsoft Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365 pentru prima dată, memoria cache de supranume (stocată în fișierul .nk2 numele de profil) este importată într-un mesaj ascuns din magazinul de mesaje implicit.

Pentru a importa fișiere .nk2 în Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365, asigurați-vă că fișierul .nk2 se află în următorul folder: %appdata%\Microsoft\Outlook

**Notă:** fișierul .nk2 trebuie să aibă același nume ca cel al fișierului dvs. Outlook 2013 sau Outlook 2016 date. În mod implicit, numele profilului este "Outlook". Pentru a verifica numele profilului, urmați acești pași: 
1. Faceți **clic pe Start,** apoi pe **Panou de control.**
2. Faceți dublu clic pe **Corespondență.**
3. În caseta de dialog Inițializare corespondență, selectați **Afișare profiluri.**
4. Selectați **Start**  >  **Executare**.
5. În caseta **Deschidere,** tastați *outlook.exe /importnk2*, apoi selectați **OK.** 

După ce importați fișierul .nk2, conținutul fișierului este îmbinat în memoria cache de supranume existentă, stocată în cutia poștală.

**Notă:** Fișierul .nk2 este redenumit cu o extensie de nume de fișier .old data viitoare când începeți Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365. Dacă doriți să importați din nou fișierul .nk2, eliminați mai întâi extensia .old nume de fișier.

Pentru mai multe informații, [consultați Importul sau copierea Listei completare automată pe alt computer.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)