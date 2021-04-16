---
title: 0x8004de40 la lansarea OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813664"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 la lansarea OneDrive

Dacă primiți un mesaj de eroare **0x8004de40** atunci când vă conectați la OneDrive, reporniți computerul în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală. Dacă primiți această eroare după repornire, încercați aceasta în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală:

1. Faceți clic pe Start și **tastați cmd** sau **linie** de comandă în caseta de căutare, faceți clic dreapta pe aplicația linie de comandă și **selectați Rulare ca administrator.** Dacă vi se solicită o parolă de administrator sau o confirmare, tastați parola sau faceți clic pe **Se permite**.  

2. În fereastra Linie de comandă, tastați **dsregcmd /leave și**  așteptați să se termine comanda. Apoi tastați **dsregcmd /join** și așteptați comanda să se termine.
3. Reporniți computerul.
