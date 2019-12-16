---
title: E-mailul fluxului de lucru nu este trimis
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049385"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail de flux de lucru nu este trimis pentru o listă SharePoint sau bibliotecă

1. E-mailurile din fluxuri de lucru nu sunt trimise tuturor utilizatorilor sau numai utilizatorilor specifici sau vedeți eroarea **mesajul de poștă electronică nu poate fi trimis. Asigurați-vă că poșta electronică are un destinatar valid**.

    Verificați dacă utilizatorul există în grupul de permisiuni **toate persoanele** (lista de informații de utilizator) pentru acea colecție de site-uri.  Exemplu de URL direct:<tenant>https://.<sitename>SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat în pagină. 
    - Dacă este un utilizator extern, asigurați-vă că invitația lor a fost acceptată.
    - Dacă utilizatorul există în grupul de permisiuni, asigurați-vă că adresa de e-mail este corectă.
    - Dacă adresa de e-mail a utilizatorilor nu este setată aici, apoi creați o alertă de eșantion pentru acel utilizator care obligă sincronizarea acelui cont de utilizator din profilurile de utilizator ale SharePoint la această colecție de site-uri.
 
2. E-mailul din fluxurile de lucru sunt trimise administratorilor de colecție de site-uri, dar nu și altor utilizatori și vedeți eroarea **http interzisă la <span>https:</span>//_vti_bin/client.XVC.SP.Utilities.Utility.SendEmail**.
 

    Consultați [acces refuzat atunci când trimiteți un e-mail la un grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    De asemenea, Verificați că caracteristica de colectare a site-ului de **blocare permisiuni de acces limitat de utilizator** nu este activă.


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


