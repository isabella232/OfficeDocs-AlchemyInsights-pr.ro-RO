---
title: 1491-căutare-nu-returnare-așteptat-rezultate
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709239"
---
# <a name="content-search-not-returning-expected-results"></a>Căutare conținut nu returnează rezultatele așteptate

Atunci când executați căutări de conținut din Centrul de securitate Microsoft 365 & conformitate, este posibil să primiți rezultate neașteptate de căutare. Luați în considerare următoarele lucruri care pot afecta rezultatele căutării:

- **Locații de conținut și condiții de căutare**: Asigurați-vă că ați selectat locațiile corespunzătoare ale conținutului și condițiile de căutare. Dacă ați efectuat o căutare amplă (cu multe locații), luați în considerare împărțirea acesteia în mai multe căutări.

- **Elemente parțial indexate:** [Elementele parțial indexate](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) din cutiile poștale sunt incluse în rezultatele căutării estimate. Cu toate acestea, elementele parțial indexate de pe site-uri din SharePoint și OneDrive nu sunt incluse în estimarea de căutare.

- **Erori de căutare**: Când căutați un număr mare de cutii poștale (peste 100.000 de cutii poștale), este posibil să obțineți erori de căutare, cu coduri de eroare, ar fi CS008-009 și CS012-002). În acest caz, încercați din nou căutarea numai pentru locațiile de conținut nereușite. Consultați [acest articol](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pentru mai multe informații.
