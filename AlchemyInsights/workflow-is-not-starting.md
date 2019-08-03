---
title: Flux de lucru nu este de plecare
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
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171805"
---
# <a name="workflow-is-not-starting"></a>Flux de lucru nu este de plecare

- Fluxuri de lucru SharePoint 2010 şi SharePoint 2013 nu incep.

    În cazul în care nu începe fluxul de lucru, poate fi o problemă temporară de serviciu în cazul în care utilizatorii pot experienţă întârzieri intermitentă cu progresul de flux de lucru. Verifica [Serviciul sănătate tabloul de bord](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) pentru a vedea dacă organizaţia dumneavoastră este afectat.

    În cazul în care mai mult de 24 de ore au trecut de când aţi văzut prima dată această problemă, vă rugăm să vă un bilet de sprijin. În multe cazuri, lucrăm deja la o soluţie. Vă rugăm să ne dea cel puţin 24 de ore pentru a finaliza o soluţie.

- Fluxuri de lucru SharePoint 2010 întârziat pe start.

    Acest lucru se întâmplă în cazul în care fluxul de lucru este declanşată în loturi mari. (de exemplu, când mai multe elemente se adaugă la o dată).

    Fluxurile de lucru nu sunt concepute pentru a rula în timp real, astfel încât o întârziere este comportamentul de design.

    În cazul în care fluxul de lucru este complex extensibil obiect Markup Language (XMOL), compilaţie poate fi lent. Verificaţi [acest](https://support.microsoft.com/en-us/kb/3043697) articol.

    Ar simplifica fluxul de lucru sau redesign-l utilizând tipul de platforma Microsoft SharePoint 2013 de flux de lucru.

    De asemenea, în cazul în care istoricul de flux de lucru a crescut mare, poate doriţi să purge elementele sau creați o listă nouă de istorie.

    Mai multe informaţii: [epurare istorie de flux de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Subiecte asociate
Doriţi să încercaţi Micrsoft fluxul în SharePoint Online?
- [Crea fluxul](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint şi fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


