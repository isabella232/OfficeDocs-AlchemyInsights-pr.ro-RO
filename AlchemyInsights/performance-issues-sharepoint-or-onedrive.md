---
title: Probleme de performanță-SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068426"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint sau OneDrive lent, inaccesibil sau indisponibil pentru mai mulți utilizatori

SharePoint sau OneDrive poate fi lent, inaccesibil sau indisponibil, sau poate afișa Serviciu indisponibil sau 503 erori, din mai multe motive:
  
- Dacă site-ul SharePoint sau OneDrive este lent sau întârziat pentru mai mulți utilizatori, poate exista o problemă de serviciu temporar în cazul în care utilizatorii experimenta întârzieri intermitente sau erori de navigare la accesarea site-uri SharePoint sau OneDrive. Verificați [tabloul de bord sănătate Service](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.
  
- Utilizatorii pot primi un *server 503 este ocupat* de eroare atunci când încercați să navigați la site-uri SharePoint sau OneDrive. Această eroare poate fi cauzată de limitare în cadrul serviciului SharePoint. SharePoint Online utilizează supraîncărcarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online. Limitare limitează numărul de acțiuni de utilizator sau apeluri simultane (prin script sau cod) pentru a preveni utilizarea excesivă a resurselor. Pentru mai multe informații despre limitare a se vedea, [evitați obtinerea limitate sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Dacă întâmpinați performanțe lente cu un site sau o pagină SharePoint **clasică** sau **modernă** , utilizați [Instrumentul de diagnosticare](https://aka.ms/perftool) a paginilor pentru a analiza paginile.
  
- Dacă încă vă confruntați cu performanțe lente generale, vă rugăm să revizuiți resursele din partea de jos a acestui articol: [Introducere în reglarea performanței pentru SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  