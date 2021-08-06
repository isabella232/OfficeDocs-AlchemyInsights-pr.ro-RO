---
title: Fluxul de lucru nu porni
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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907750"
---
# <a name="workflow-is-not-starting"></a>Fluxul de lucru nu porni

- SharePoint 2010 și SharePoint 2013 nu încep.

    - Dacă fluxul dvs. de lucru nu începe, poate exista o problemă temporară de serviciu în care utilizatorii se pot experimenta întârzieri intermitente în progresul fluxului de lucru. Verificați tabloul [de bord cu starea](https://admin.microsoft.com/AdminPortal/Home/servicehealth) serviciilor pentru a vedea dacă organizația dvs. este afectat.

    - Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să introduceți în jurnal un tichet de asistență. În multe cazuri, lucrăm deja la o soluție. Acordați-ne cel puțin 24 de ore pentru a finaliza o soluție.

- SharePoint 2010 a întârziat la pornire.

    - Acest lucru se întâmplă dacă fluxul de lucru este declanșat în grupuri mari. (de exemplu, când se adaugă mai multe elemente simultan).

    - Fluxurile de lucru nu sunt proiectate pentru a rula în timp real, astfel că o întârziere este un comportament prin proiectare.

   -  Dacă Fluxul de lucru este un limbaj X SCURT (Extensible Object Markup Language), compilarea poate fi lentă. Consultați [acest](https://support.microsoft.com//kb/3043697) articol.

    - Trebuie să simplificați fluxul de lucru sau să-l reproiectați utilizând tipul de platformă de flux de lucru Microsoft SharePoint 2013.

    - Dacă istoricul fluxului de lucru s-a dezvoltat, se poate să doriți să goliți elementele sau să creați o nouă listă de istoric.

        Mai multe informații: [Goliți istoricul fluxului de lucru](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Crearea Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
