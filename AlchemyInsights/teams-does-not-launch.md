---
title: Teams nu se lansează
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813356"
---
# <a name="teams-doesnt-launch"></a>Teams nu se lansează

Dacă încercați să deschideți un Microsoft Teams se lansează niciodată, încercați următoarele:

1. Navigați **la %appdata%\Microsoft\Teams**.
1. Ștergeți conținutul folderului.
1. Reporniți computerul și încercați să lansați o Teams.

Poate fi necesar să reinstalați Teams. Pentru a reinstala:

1. Dezinstalați Teams utilizând Panoul de control.
1. Navigați **la %appdata%\Microsoft\Teams\Application Cache**.
1. Ștergeți conținutul folderului.
1. Navigați **la %appdata%\Microsoft\teams\Cache**.
1. Ștergeți conținutul folderului.
1. Reporniți computerul, apoi descărcați și instalați Teams.

Dacă doriți să rulați un diagnostic în entitatea dvs. găzduită pentru un anumit utilizator care nu se poate conecta, începeți o căutare nouă cu cuvântul cheie **TeamsUserUnableToSignIn** și urmați instrucțiunile.