---
title: Restricționarea SharePoint Online la modul clasic
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742481"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Restricționarea SharePoint Online la modul clasic

Unele organizații necesită în continuare experiența modului clasic. Deși nu există planuri de eliminare a modului clasic la un nivel granular, nu mai este posibil să restricționați o întreagă organizație (entitate găzduită) la modul clasic pentru liste și biblioteci.

Administratorul va avea următoarele opțiuni pentru a gestiona listele și bibliotecile individuale în modul clasic utilizând comutatoare de renunțare granulare pe care le oferim la următoarele niveluri:

- colecție de site-uri
- Site
- Listă
- Biblioteca

În plus, listele care utilizează anumite caracteristici și particularizări care nu sunt acceptate de modern va fi în continuare automat comutate la modul clasic.

Începând cu 1 aprilie 2019, procesul de dezactivare a nivelului de entitate găzduită renunță la lista modernă, iar bibliotecile vor începe și vor continua până la 31 mai 2019.  Listele și bibliotecile care se află în modul clasic ca urmare a excluderii pentru entitate găzduită vor fi mutate automat la modern.

Dacă aveți nevoie de modul clasic, vă rugăm să consultați mai multe informații [aici](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) și instrucțiuni Powershell PnP [aici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) care descrie opțiunile și instrumentele pe care le puteți utiliza astăzi pentru a utiliza experiența modului clasic.
