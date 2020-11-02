---
title: eroare 0x8004de40 atunci când lansați OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823115"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>eroare 0x8004de40 atunci când lansați OneDrive

Dacă primiți o eroare **0x8004de40** atunci când vă conectați la OneDrive, reporniți computerul în timp ce sunteți conectat la locul de muncă sau de la școală. Dacă primiți această eroare după repornirea acestuia, încercați acest lucru în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală:

1. Faceți clic pe Start și tastați **cmd** sau **promptul de comandă**  în caseta de căutare, faceți clic cu butonul din dreapta pe aplicația linie de comandă și selectați  **rulare ca administrator** . Dacă vi se solicită o parolă de administrator sau o confirmare, tastați parola sau faceți clic pe se **permite** .  

2. În fereastra linie de comandă, tastați **dsregcmd/Leave**  și așteptați ca comanda să se termine. Apoi tastați **dsregcmd/Join** și așteptați ca comanda să se termine.
3. Reporniți computerul.
