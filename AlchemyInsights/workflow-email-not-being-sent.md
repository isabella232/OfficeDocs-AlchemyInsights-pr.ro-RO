---
title: E-mailul fluxului de lucru nu se trimite
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
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072532"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mailul fluxului de lucru nu este trimis pentru o SharePoint sau o bibliotecă

1. E-mailurile de la fluxurile de lucru nu sunt trimise tuturor utilizatorilor sau doar anumitor utilizatori sau vedeți eroarea Mesajul de e-mail nu poate fi **trimis. Asigurați-vă** că mesajul de e-mail are un destinatar valid.

    Verificați dacă utilizatorul există în grupul de permisiuni **Toate persoanele** (lista de informații utilizator) pentru acea colecție de site-uri.  Url direct eșantion: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat la pagină. 
    - Dacă este un utilizator extern, asigurați-vă că invitația sa a fost acceptată.
    - Dacă utilizatorul există în grupul de permisiuni, asigurați-vă că adresa de e-mail este corectă.
    - Dacă adresa de e-mail a utilizatorilor nu este setată aici, creați o avertizare eșantion pentru acel utilizator, care forțează sincronizarea contului de utilizator respectiv din Profiluri de utilizator SharePoint la această colecție de site-uri.
 
2. E-mailurile de la fluxurile de lucru sunt trimise administratorilor colecției de site-uri, dar nu altor utilizatori și vedeți eroarea **HTTP Forbidden la <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Consultați [Acces refuzat atunci când trimiteți un mesaj de e-mail la un grup SharePoint .](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    De asemenea, verificați dacă nu este activă caracteristica de blocare a **permisiunii** utilizatorului cu acces limitat.


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Crearea Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


