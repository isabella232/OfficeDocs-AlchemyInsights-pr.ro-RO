---
title: Fluxul de lucru nu pornește
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738101"
---
# <a name="workflow-is-not-starting"></a>Fluxul de lucru nu pornește

- SharePoint 2010 și SharePoint 2013 fluxuri de lucru nu pornesc.

    - Dacă fluxul de lucru nu pornește, este posibil să existe o problemă de serviciu temporară în care utilizatorii pot experimenta întârzieri intermitente cu progresul fluxului de lucru. Verificați [tabloul de bord sănătate Service](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizația este afectată.

    - Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un bilet de suport. În multe cazuri, suntem deja de lucru pe o soluție. Vă rugăm să ne acordați cel puțin 24 de ore pentru a finaliza o soluție.

- Fluxurile de lucru SharePoint 2010 întârziate la pornire.

    - Acest lucru se întâmplă dacă fluxul de lucru este declanșat în loturi mari. (de exemplu, atunci când mai multe elemente sunt adăugate la o dată).

    - Fluxurile de lucru nu sunt proiectate să ruleze în timp real, astfel încât o întârziere este un comportament de proiectare.

   -  Dacă fluxul de lucru este complex extensibil obiect Markup Language (XMOL), compilarea poate fi lentă. Verificați [acest](https://support.microsoft.com//kb/3043697) articol.

    - Trebuie să Simplificați fluxul de lucru sau să îl reproiectați utilizând tipul platformei Microsoft SharePoint 2013 Workflow.

    - Dacă Istoricul fluxului de lucru a crescut mare, este posibil să doriți să curățați elementele sau să creați o nouă listă de istoric.

        Mai multe informații: [golirea istoricului fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


