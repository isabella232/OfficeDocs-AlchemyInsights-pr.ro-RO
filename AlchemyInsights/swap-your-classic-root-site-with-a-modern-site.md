---
title: Swap site-ul rădăcină clasic cu un site modern
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749272"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap site-ul rădăcină clasic cu un site modern

Dacă mediul a fost configurat înainte de aprilie 2019, aveți posibilitatea să modificați site-ul rădăcină la un site modern utilizând Microsoft PowerShell:

- Dacă aveți un site diferit pe care doriți să-l utilizați ca site-ul rădăcină, puteți înlocui [(swap) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu ea. 
    - Utilizați [Invoke-,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil pentru ambele site-uri de echipă (nu sunt conectate la un grup) și site-ul de comunicare. 

- Capacitățile suplimentare vor fi introduse în curând, care vă va permite să păstrați folosind conținutul de pe site-ul, dar converti site-ul existent la un site de comunicare. 
>[!Important]
>Aceste capacități vor fi laminate treptat. Continuați pentru a verifica Office 365 Message Center pentru actualizări. 

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu schimbarea site-uri

- Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie scotocit din nou pentru a actualiza indexul de căutare. Nu există nici un pas manual necesar-acest lucru se va face în mod automat.
- Orice depinde de "static" link-uri (cum ar fi fișiere de sincronizare și fișiere OneNote) va trebui să fie corectate manual.
- Dacă site-ul sursă a fost un site de știri organizaționale, actualizați URL-ul.Obțineți o listă cu toate site-urile de știri organizatorice.
- Site-uri de proiect Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect.





