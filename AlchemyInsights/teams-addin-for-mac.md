---
title: Programul de completare teams pentru Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629827"
---
# <a name="teams-add-in-for-mac"></a>Programul de completare teams pentru Mac

Pentru a depana un program de completare teams care lipsește pentru utilizatorii sistemului de operare Mac, urmați acești pași:

**Pasul 1:** Dacă aveți Exchange hibrid local (2016 CU3 sau o versiune mai recentă), utilizați instrumentul de Test-HMA.ps1 pentru a confirma că autentificarea modernă hibridă este configurată corect. Pentru mai multe informații, consultați [validarea instalării hibride moderne de autentificare pentru Outlook pentru iOS și Android](https://aka.ms/AA980zq).  

**Notă** Utilizați formatul de adresă UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)), nu domain\username. Faceți acest lucru chiar și pentru utilizatorii cu cutii poștale Exchange Online.

**Pasul 2:** Să aibă utilizatorul Accesați conturile de **Instrumente**  >  **Accounts**... în Outlook pentru Mac și găsiți și selectați contul. Confirmați numele de utilizator listat este în format UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)).

**Pasul 3:** Confirmați că utilizatorul este un utilizator Microsoft teams licențiat. Utilizatorul trebuie să utilizeze abonamentul Office 365 pentru Mac, versiunea de produs 16,24 sau o versiune mai recentă.