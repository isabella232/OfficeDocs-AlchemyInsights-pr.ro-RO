---
title: 1491-căutare-nu-returnare-așteptat-Rezultate
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740486"
---
# <a name="content-search-not-returning-expected-results"></a>Căutarea de conținut nu returnează rezultatele așteptate

Atunci când se execută căutări de conținut din centrul de conformitate Microsoft 365 Security &, este posibil să primiți rezultate neașteptate de căutare. Luați în considerare următoarele lucruri care vă pot afecta rezultatele căutării:

- **Locații de conținut și condiții de căutare**: Asigurați-vă că ați selectat locațiile de conținut corespunzătoare și condițiile de căutare. Dacă ați rulat o căutare mare (cu multe locații), luați în considerare împărțirea acesteia în mai multe căutări.

- **Elemente indexate parțial**:  [elementele indexate parțial](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) din cutiile poștale sunt incluse în rezultatele de căutare estimate. Cu toate acestea, elementele indexate parțial din site-uri în SharePoint și OneDrive nu sunt incluse în estimarea de căutare.

- **Erori de căutare**: atunci când căutați un număr mare de cutii poștale (peste 100.000 de cutii poștale), este posibil să primiți erori de căutare, cu coduri de eroare, cum ar fi CS008-009 și CS012-002). În acest caz, încercați din nou căutarea doar pentru locațiile de conținut nereușite. Pentru mai multe informații, consultați  [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
