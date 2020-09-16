---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771913"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint sau OneDrive este lent, inaccesibil sau indisponibil pentru mai mulți utilizatori

SharePoint sau OneDrive pot fi lente, inaccesibile sau indisponibile sau pot afișa erorile de serviciu indisponibile sau 503, din mai multe motive:
  
- Dacă site-ul SharePoint sau OneDrive este lent sau întârziat pentru mai mulți utilizatori, este posibil să existe o problemă de serviciu temporară în care utilizatorii întâmpină întârzieri intermitente sau erori de navigare atunci când accesează site-uri SharePoint sau conținut OneDrive. Verificați [tabloul de bord stare servicii](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.
  
- Utilizatorii pot primi un *server 503 este o eroare ocupată* atunci când încercați să navigați la site-uri SharePoint sau OneDrive. Această eroare poate fi cauzată de limitarea în serviciul SharePoint. SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online. Limitarea se aplică la numărul de acțiuni de utilizator sau apeluri concurente (după script sau cod), pentru a preveni utilizarea excesivă a resurselor. Pentru mai multe informații despre limitare, consultați [evitați să fiți accelerat sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Dacă vă confruntați cu o performanță lentă cu un site sau o pagină SharePoint **clasică** sau **modernă** , utilizați [Instrumentul de diagnosticare](https://aka.ms/perftool) a paginilor pentru a analiza paginile.
  
- Dacă încă întâmpinați performanțe generale lente, consultați resursele din partea de jos a acestui articol: [Introducere în ajustarea performanței pentru SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  