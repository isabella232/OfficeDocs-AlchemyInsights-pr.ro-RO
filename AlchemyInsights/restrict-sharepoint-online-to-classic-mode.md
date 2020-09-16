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
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751434"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restricționarea SharePoint Online la modul clasic

Unele organizații necesită încă experiența modul clasic. Deși nu există planuri pentru a elimina modul clasic la un nivel granular, nu mai este posibil să restricționați o întreagă organizație (entitate găzduită) la modul clasic pentru liste și biblioteci.

Administratorul va avea următoarele opțiuni pentru a gestiona listele și bibliotecile individuale în modul clasic, utilizând argumentele de renunțare granulare pe care le oferim la următoarele niveluri:

- colecția de site-uri
- site
- listă
- Bibliotecă

În plus, listele care utilizează anumite caracteristici și particularizări care nu sunt acceptate de modern vor fi în continuare automat comutate în modul clasic.

Începând cu 1 aprilie 2019, procesul de dezactivare a nivelului de entitate găzduită renunțați la lista modernă și bibliotecile vor începe și vor continua până la 31 mai 2019.  Listele și bibliotecile care se află în modul clasic ca rezultat al renunțării la entitatea găzduită vor fi transferate automat la modern.

Dacă aveți nevoie de modul clasic, vă rugăm să vedeți mai multe informații [aici](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) și instrucțiuni pentru PNP PowerShell [aici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , care descrie opțiunile și instrumentele pe care le puteți utiliza astăzi pentru a utiliza experiența mod clasic.
