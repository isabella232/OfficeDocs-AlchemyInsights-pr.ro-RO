---
title: 1491-search-not-return-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052722"
---
# <a name="content-search-not-returning-expected-results"></a>Căutarea conținutului nu întoarce rezultatele așteptate

Atunci când rulați căutări de conținut din Centrul Microsoft 365 de & conformitate, este posibil să primiți rezultate de căutare neașteptate. Luați în considerare următoarele lucruri care vă pot afecta rezultatele căutării:

- **Locații de conținut și condiții de căutare:** Asigurați-vă că ați selectat locațiile de conținut și condițiile de căutare corespunzătoare. Dacă aveți o căutare mare (cu multe locații), luați în considerare scindarea sa în mai multe căutări.

- **Elemente indexate parțial:** Elementele  [indexate parțial din cutiile](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) poștale sunt incluse în rezultatele de căutare estimate. Totuși, elementele indexate parțial din site-SharePoint și OneDrive nu sunt incluse în estimarea de căutare.

- Erori **de** căutare: Atunci când căutați într-un număr mare de cutii poștale (peste 100.000 de cutii poștale), este posibil să obțineți erori de căutare, cu coduri de eroare cum ar fi CS008-009 și CS012-002). În acest caz, reîncercați căutarea numai pentru locațiile de conținut nereușit. Consultați  [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) pentru mai multe informații.
