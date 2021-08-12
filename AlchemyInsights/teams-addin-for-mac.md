---
title: Teams de completare pentru Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940687"
---
# <a name="teams-add-in-for-mac"></a>Teams de completare pentru Mac

Pentru a depana un Teams de completare pentru utilizatorii sistemului de operare Mac, urmați acești pași:

**Pasul 1:** Dacă aveți autentificare hibridă Exchange (2016 CU3 sau o versiune mai recentă), utilizați instrumentul Test-HMA.ps1 pentru a confirma că autentificarea modernă hibridă este configurată corect. Pentru mai multe informații, [consultați Validarea configurării de autentificare modernă hibridă pentru Outlook pentru iOS și Android.](https://aka.ms/TestHMAEAS)  

**Notă** Utilizați formatul DE ADRESĂ UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)), nu domeniul \numeutilizator. Faceți acest lucru chiar și pentru utilizatorii Exchange Online poștale.

**Pasul 2:** Spuneți utilizatorului să meargă **la Conturi**  >  **instrumente...** în Outlook pentru Mac și găsiți și selectați contul. Confirmați că numele de utilizator listat este în format UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)).

**Pasul 3:** Confirmați că utilizatorul este utilizator cu Microsoft Teams licențe. Utilizatorul trebuie să folosească abonamentul Office 365 Mac, versiunea de produs 16.24 sau o versiune mai recentă.