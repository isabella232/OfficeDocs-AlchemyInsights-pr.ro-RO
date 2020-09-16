---
title: Programul de completare teams pentru Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670340"
---
# <a name="teams-add-in-for-mac"></a>Programul de completare teams pentru Mac

Pentru a depana un program de completare teams care lipsește pentru utilizatorii sistemului de operare Mac, urmați acești pași:

**Pasul 1:** Dacă aveți Exchange hibrid local (2016 CU3 sau o versiune mai recentă), utilizați instrumentul de Test-HMA.ps1 pentru a confirma că autentificarea modernă hibridă este configurată corect. Pentru mai multe informații, consultați [validarea instalării hibride moderne de autentificare pentru Outlook pentru iOS și Android](https://aka.ms/AA980zq).  

**Notă** Utilizați formatul de adresă UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)), nu domain\username. Faceți acest lucru chiar și pentru utilizatorii cu cutii poștale Exchange Online.

**Pasul 2:** Să aibă utilizatorul Accesați conturile de **Instrumente**  >  **Accounts**... în Outlook pentru Mac și găsiți și selectați contul. Confirmați numele de utilizator listat este în format UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)).

**Pasul 3:** Confirmați că utilizatorul este un utilizator Microsoft teams licențiat. Utilizatorul trebuie să utilizeze abonamentul Office 365 pentru Mac, versiunea de produs 16,24 sau o versiune mai recentă.