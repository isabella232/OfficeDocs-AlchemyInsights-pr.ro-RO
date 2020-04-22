---
title: Fluxul de lucru nu pornește
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766109"
---
# <a name="workflow-is-not-starting"></a>Fluxul de lucru nu pornește

- Fluxurile de lucru SharePoint 2010 și SharePoint 2013 nu pornesc.

    - Dacă fluxul de lucru nu pornește, este posibil să existe o problemă de serviciu temporar în cazul în care utilizatorii pot apărea întârzieri intermitente cu progresul fluxului de lucru. Verificați [Tabloul de bord de sănătate serviciu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.

    - Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să vă conectați un bilet de asistență. În multe cazuri, lucrăm deja la o soluție. Vă rugăm să ne dea cel puțin 24 de ore pentru a finaliza o soluție.

- Fluxuri de lucru SharePoint 2010 întârziate la pornire.

    - Acest lucru se întâmplă dacă fluxul de lucru este declanșat în loturi mari. (de exemplu, atunci când mai multe elemente sunt adăugate simultan).

    - Fluxurile de lucru nu sunt proiectate să ruleze în timp real, deci o întârziere este comportamentul de proiectare.

   -  Dacă fluxul de lucru este complex Extensible Object Markup Language (XMOL), compilarea poate fi lentă. Verificați [acest](https://support.microsoft.com//kb/3043697) articol.

    - Ar trebui să simplificați fluxul de lucru sau să îl reproiectați utilizând tipul de platformă Microsoft SharePoint 2013 Flux de lucru.

    - Dacă istoricul fluxului de lucru a crescut, se recomandă să goliți elementele sau să creați o listă de istoricnou.

        Informații suplimentare: [Golire istoric flux de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


