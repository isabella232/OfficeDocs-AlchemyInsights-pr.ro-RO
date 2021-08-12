---
title: Transferarea site-ului rădăcină clasic cu un site modern
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
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940831"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Transferarea site-ului rădăcină clasic cu un site modern

Dacă mediul dvs. a fost configurat înainte de aprilie 2019, puteți schimba site-ul rădăcină într-un site modern, utilizând Microsoft PowerShell:

- Dacă aveți un alt site pe care doriți să-l utilizați ca site rădăcină, puteți înlocui [(înlocui) site-ul rădăcină](https://docs.microsoft.com/sharepoint/modern-root-site) cu acesta. 
    - Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a transfera locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil atât pentru site-ul de echipă (neconectat la un grup), cât și pentru Site-ul de comunicare. 

- În curând vor fi introduse capacități suplimentare care vă vor permite să continuați să utilizați conținutul de pe site, dar să efectuați conversia site-ului existent la un site de comunicare. 
>[!Important]
>Aceste capacități vor fi integrate treptat. Continuați să verificați Centrul de mesaje pentru actualizări. 

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu comutarea între site-uri

- Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie resuficat pentru a actualiza indexul de căutare. Nu este necesar niciun pas manual - acest lucru se va face automat.
- Orice legătură dependentă de linkurile "statice" (cum ar fi Sincronizare fișier OneNote fișiere) va trebui corectată manual.
- Dacă site-ul sursă a fost un site de știri organizațional, actualizați URL-ul. Obțineți o listă cu toate site-urile de știri organizaționale.
- Project Site-urile server pot avea nevoie să fie validate, pentru a vă asigura că sunt în continuare asociate corect.
