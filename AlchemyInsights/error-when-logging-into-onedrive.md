---
title: 0x8004de40 eroare la lansarea unei OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946591"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 eroare la lansarea unei OneDrive

Dacă primiți un mesaj de eroare **0x8004de40** vă conectați la OneDrive, reporniți computerul în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală. Dacă primiți această eroare după repornire, încercați aceasta în timp ce sunteți conectat la domeniul de la locul de muncă sau de la școală:

1. Faceți clic pe Start și **tastați cmd** sau **linie** de comandă în caseta de căutare, faceți clic dreapta pe aplicația linie de comandă și **selectați Rulare ca administrator.** Dacă vi se solicită o parolă de administrator sau o confirmare, tastați parola sau faceți clic pe **Se permite**.  

2. În fereastra Linie de comandă, tastați **dsregcmd /leave și**  așteptați să se termine comanda. Apoi tastați **dsregcmd /join** și așteptați comanda să se termine.
3. Reporniți computerul.
