---
title: Adresarea erorii de conectare Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821999"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresarea erorii de conectare Teams AADSTS9000411

Atunci când vă conectați la Microsoft Teams, este posibil să primiți eroarea: Ne pare rău, dar avem probleme cu conectarea dvs. la **AADSTS9000411: Solicitarea nu este formatată corect. Parametrul "login_hint" este dublat.**

Pentru a rezolva această problemă, asigurați-vă că clienții Microsoft Teams sunt actualizați. Pentru mai multe informații despre actualizarea clientului, consultați [Actualizarea Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Dacă nu puteți actualiza clientul dintr-un anumit motiv, deconectarea de la client va șterge majoritatea datelor memorate în cache. Cu toate acestea, dacă aveți încă probleme după logoff/logon, închideți Teams și goliți memoria cache a clientului, în modul următor:
1. Închideți Microsoft Teams.
2. Accesați: %appdata%\microsoft\teams și ștergeți toate fișierele.
3. Redeschideți Microsoft Teams.
