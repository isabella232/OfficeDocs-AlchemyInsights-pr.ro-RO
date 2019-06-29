---
title: 1491-Search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355889"
---
# <a name="content-search-not-returning-expected-results"></a>Căutare conţinutul nu returna rezultatele aşteptate

Atunci când rulează conţinut căutări din Office 365 securitate & centru de conformitate, puteţi primi rezultate neaşteptate. Luaţi în considerare următoarele lucruri care pot afecta rezultatele căutării:

- **Locaţii de conţinut şi condiţiile de căutare**: Asiguraţi-vă că aţi selectat locatiile conţinut adecvat şi condiţii de căutare. Dacă aţi rulat o căutaţi mare (cu mai multe locaţii), ia în considerare o diviza în mai multe căutări.

- **Parţial indexat articole**: [parţial indexate elementele](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) din cutiile poştale sunt incluse în rezultatele de căutare estimată. Cu toate acestea, parţial indexate elemente din site-urile SharePoint și OneDrive nu sunt incluse în estimarea de căutare.

- **Eşecuri de căutare**: atunci când caută un număr mare de cutii poştale (peste 100.000 poştale), este posibil să primiţi erori de căutare, cu codurile de eroare, cum ar fi CS008-009 si CS012-002). În acest caz, încercaţi din nou căutare doar pentru locatii de conţinut nu a reuşit. A se vedea [acest articol](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pentru mai multe informaţii.
