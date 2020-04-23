---
title: Schimbați-vă site-ul rădăcină clasic cu un site modern
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741556"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Schimbați-vă site-ul rădăcină clasic cu un site modern

Dacă mediul a fost configurat înainte de aprilie 2019, puteți modifica site-ul rădăcină într-un site modern utilizând Microsoft PowerShell:

- Dacă aveți un alt site pe care doriți să îl utilizați ca site rădăcină, puteți înlocui [(schimba) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu acesta. 
    - Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil atât pentru site-ul de echipă (care nu este conectat la un grup), cât și pentru site-ul de comunicare. 

- Capacități suplimentare vor fi introduse în curând, care vă vor permite să continuați să utilizați conținutul de pe site, dar să convertiți site-ul existent într-un site de comunicare. 
>[!Important]
>Aceste capabilități vor fi lansate treptat. Continuați să verificați Centrul de mesaje pentru actualizări. 

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu site-uri de schimbare

- Site-ul țintă poate returna o eroare "negăsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui recrawled pentru a actualiza indexul de căutare. Nu există nici un pas manual necesar - acest lucru se va face în mod automat.
- Orice lucru dependent de linkurile "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui corectat manual.
- Dacă site-ul sursă a fost un site de știri organizațional, actualizați URL-ul.Obțineți o listă cu toate site-urile de știri organizaționale.
- Site-uri Project Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.
