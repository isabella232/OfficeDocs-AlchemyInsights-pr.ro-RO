---
title: Probleme de performanță SharePoint sau OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911854"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint sau OneDrive lentă, inaccesibilă sau indisponibilă pentru mai mulți utilizatori

SharePoint sau OneDrive pot fi lente, inaccesibile sau indisponibile sau pot afișa servicii indisponibile sau 503 erori din mai multe motive:
  
- Dacă site-ul dvs. SharePoint sau OneDrive este lent sau întârziat pentru mai mulți utilizatori, poate exista o problemă temporară de serviciu în care utilizatorii experimentează întârzieri intermitente sau erori de navigare atunci când accesează site-uri SharePoint-uri OneDrive conținut. Verificați tabloul [de bord Starea serviciilor](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația dvs. este afectat.
  
- Utilizatorii pot primi o *eroare de tip server 503* sunt ocupați atunci când încearcă să navigheze la site-SharePoint-uri OneDrive date. Această eroare poate fi cauzată de o throtare din serviciul SharePoint date. SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online. Limitarea se aplică la numărul de acțiuni de utilizator sau apeluri concurente (după script sau cod), pentru a preveni utilizarea excesivă a resurselor. Pentru mai multe informații despre reglare, consultați Evitați a se regla sau bloca [în SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Dacă vă experimentați o performanță lentă **cu** un site **sau** o pagină SharePoint clasică sau modernă, utilizați instrumentul [Diagnosticare pagină](https://aka.ms/perftool) pentru a analiza paginile.
  
- Dacă încă vă așteptați la o performanță generală lentă, consultați resursele din partea de jos a acestui articol: Introducere în ajustarea [performanței SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  