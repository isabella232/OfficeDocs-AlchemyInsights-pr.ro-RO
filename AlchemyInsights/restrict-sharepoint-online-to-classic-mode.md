---
title: Restricționarea SharePoint Online la modul clasic
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958813"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restricționarea SharePoint Online la modul clasic

Unele organizații necesită în continuare experiența modului Clasic. Deși nu există planuri pentru a elimina modul clasic la nivel de granular, nu mai este posibil să restricționați o întreagă organizație (entitate găzduită) la modul clasic pentru liste și biblioteci.

Administratorul va avea următoarele opțiuni pentru a gestiona listele și bibliotecile individuale în modul clasic, utilizând comutatoarele de renunțare granulară pe care le furnizăm la următoarele niveluri:

- colecție de site-uri
- site
- listă
- bibliotecă

În plus, listele care utilizează anumite caracteristici și particularizări ce nu sunt acceptate de versiunea modernă vor fi comutate în continuare automat la modul clasic.

Începând cu 1 aprilie 2019, procesul de dezactivare a nivelului entității găzduite va renunța la lista și bibliotecile moderne și va continua până la 31 mai 2019.  Listele și bibliotecile aflate în modul clasic ca urmare a opțiunii de renunțare la entitatea găzduită vor fi automat mutate în modul modern.

Dacă aveți nevoie de modul [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) clasic, vedeți aici [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) mai multe informații, iar instrucțiunea PnP Powershell aici care descrie opțiunile și instrumentele pe care le puteți utiliza astăzi pentru a utiliza experiența modului clasic.
