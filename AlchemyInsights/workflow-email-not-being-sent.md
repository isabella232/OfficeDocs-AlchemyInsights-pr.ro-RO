---
title: E-mailul fluxului de lucru nu este trimis
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
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766145"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mailul fluxului de lucru nu este trimis pentru o listă sau o bibliotecă SharePoint

1. E-mailul din fluxurile de lucru nu este trimis tuturor utilizatorilor sau numai anumitor utilizatori sau vedeți **eroarea Mesajul de poștă electronică nu poate fi trimis. Asigurați-vă că poșta electronică are un destinatar valid**.

    Verificați dacă utilizatorul există în grupul permisiuni **toate persoanele** (lista de informații de utilizator) pentru colecția de site-uri respectivă.  Exemplu de URL<tenant>direct: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembruGroupId=0

    - Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat la pagină. 
    - Dacă este un utilizator extern, asigurați-vă că invitația lor a fost acceptată.
    - Dacă utilizatorul există în grupul de permisiuni, asigurați-vă că adresa de e-mail este corectă.
    - Dacă adresa de e-mail a utilizatorilor nu este setată aici, creați o avertizare eșantion pentru acel utilizator care forțează sincronizarea acelui cont de utilizator din profilurile de utilizator sharepoint la această colecție de site-uri.
 
2. E-mail de la fluxuri le-a trimis administratorilor colecției de site-uri, dar nu și altor utilizatori și a vedea eroarea **HTTP Interzis la <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Consultați [Acces refuzat atunci când trimiteți un e-mail unui grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    De asemenea, verificați că caracteristica **limitată de blocare permisiuneutilizator modul de blocare** colecție de site-ul nu este activ.


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


