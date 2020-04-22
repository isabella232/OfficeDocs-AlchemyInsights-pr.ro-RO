---
title: să-import-nk2-fișiere
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759344"
---
# <a name="how-to-import-nk2-files"></a>se importă fișiere .nk2 

Când porniți Microsoft Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365 pentru prima dată, memoria cache de porecle (stocate în fișierul *profil*.nk2) este importat într-un mesaj ascuns în depozitul de mesaje implicit.

Pentru a importa fișiere .nk2 în Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365, asigurați-vă că fișierul .nk2 este în următorul folder: %appdata%\Microsoft\Outlook

**notițe:** Fișierul .nk2 trebuie să aibă același nume ca profilul Outlook 2013 sau Outlook 2016 curent. În mod implicit, numele de profil este "Outlook". Pentru a verifica numele profilului, urmați acești pași: 
1. Faceți clic pe **Start**, apoi pe **Panou de control**.
2. Faceți dublu clic pe **Mail**.
3. În caseta de dialog Configurare corespondență, selectați **Afișare profiluri**.
4. Selectați **Pornire** > **executare**.
5. În caseta **Deschidere,** tastați *outlook.exe /importnk2*, apoi selectați **OK**. 

După ce importați fișierul .nk2, conținutul fișierului sunt îmbinate în memoria cache de porecle existente stocate în cutia poștală.

**Notă:** Fișierul .nk2 este redenumit cu o extensie de nume de fișier .old la următoarea pornire Outlook 2013, Outlook 2016, Outlook 2019 sau Outlook pentru Microsoft 365. Dacă doriți să importați din nou fișierul .nk2, eliminați mai întâi extensia de nume de fișier .old.

Pentru mai multe informații, consultați [Importul sau copierea Listei de completare automată pe alt computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).