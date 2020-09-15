---
title: Swap site-ul rădăcină clasic cu un site modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691191"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap site-ul rădăcină clasic cu un site modern

Dacă mediul a fost configurat înainte de aprilie 2019, puteți să modificați site-ul rădăcină la un site modern, utilizând Microsoft PowerShell:

- Dacă aveți un alt site pe care doriți să-l utilizați ca site rădăcină, puteți înlocui [(swap) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu acesta. 
    - Utilizați [invocare-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu alt site în timp ce arhivați site-ul original. Disponibil pentru ambele site-uri de echipă (neconectat la un grup) și site de comunicare. 

- În curând vor fi introduse capacități suplimentare care vă vor permite să continuați să utilizați conținutul de pe site, dar să efectuați conversia site-ului existent pe un site de comunicare. 
>[!Important]
>Aceste capacități vor fi derulate treptat. Continuați să verificați Centrul de mesaje pentru actualizări. 

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu înlocuirea site-urilor

- Site-ul țintă poate returna o eroare "nu s-a găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie rescotocit pentru a actualiza indexul de căutare. Nu este necesar un pas manual-acest lucru se va face automat.
- Orice dependență de linkuri "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui să fie corectată manual.
- Dacă site-ul sursă a fost un site de știri organizațional, actualizați URL-ul.Obțineți o listă cu toate site-urile de știri organizaționale.
- Site-urile Project Server pot necesita validarea pentru a vă asigura că acestea sunt încă asociate corect.
