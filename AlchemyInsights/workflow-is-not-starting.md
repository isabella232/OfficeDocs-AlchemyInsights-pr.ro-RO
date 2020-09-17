---
title: Fluxul de lucru nu pornește
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794779"
---
# <a name="workflow-is-not-starting"></a>Fluxul de lucru nu pornește

- Fluxurile de lucru SharePoint 2010 și SharePoint 2013 nu pornește.

    - Dacă fluxul de lucru nu pornește, este posibil să existe o problemă de serviciu temporară, în care utilizatorii pot avea întârzieri intermitente cu progresul fluxului de lucru. Verificați [tabloul de bord stare servicii](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.

    - Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un tichet de asistență. În multe cazuri, lucrăm deja la o soluție. Vă rugăm să ne dați cel puțin 24 de ore pentru a finaliza o soluție.

- Fluxurile de lucru SharePoint 2010 au întârziat la pornire.

    - Acest lucru se întâmplă dacă fluxul de lucru este declanșat în grupuri mari. (de exemplu, atunci când sunt adăugate mai multe elemente în același timp).

    - Fluxurile de lucru nu sunt proiectate să ruleze în timp real, astfel încât o întârziere să fie un comportament de proiectare.

   -  Dacă fluxul de lucru este complex Extensible Object Markup Language (XMOL), compilarea poate fi lentă. Consultați [acest](https://support.microsoft.com//kb/3043697) articol.

    - Trebuie să Simplificați fluxul de lucru sau să îl reproiectați utilizând tipul de platformă flux de lucru Microsoft SharePoint 2013.

    - Dacă Istoricul fluxului de lucru s-a extins, se recomandă să goliți elementele sau să creați o listă de istoric nou.

        Mai multe informații: [golirea istoricului fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Crearea fluxului](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


