---
title: Adresarea echipelor de conectare eroare AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357872"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresarea echipelor de conectare eroare AADSTS9000411

Atunci când vă conectați la Microsoft Teams, este posibil să primiți eroarea: **Ne pare rău, dar avem probleme cu semnarea în AADSTS9000411: Solicitarea nu este formatat corect. Parametrul "login_hint" este duplicat.**

Pentru a rezolva această problemă, asigurați-vă că clienții Microsoft Teams sunt actualizate. Pentru mai multe informații despre actualizarea clientului, consultați [Actualizarea Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Dacă nu se poate actualiza clientul dintr-un anumit motiv, deconectarea clientului va șterge majoritatea datelor memorate în cache. Cu toate acestea, dacă aveți în continuare probleme după logoff/logon, închideți Echipe și goliți memoria cache a clientului procedând astfel:
1. Închideți Microsoft Teams.
2. Accesați: %appdata%\microsoft\teams și ștergeți toate fișierele.
3. Redeschideți Microsoft Teams.
