---
title: E-mailul fluxului de lucru nu este trimis
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749001"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mailul fluxului de lucru nu este trimis pentru o listă sau o bibliotecă SharePoint

1. E-mailul de la fluxurile de lucru nu este trimis tuturor utilizatorilor sau doar anumitor utilizatori sau vedeți eroarea **mesajul de e-mail nu poate fi trimis. Asigurați-vă că e-mailul are un destinatar valid**.

    Verificați dacă utilizatorul există în grupul permisiuni pentru **toate persoanele** (lista de informații utilizator) pentru acea colecție de site-uri.  Exemplu de URL direct: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Dacă utilizatorul nu există, asigurați-vă că utilizatorul este conectat la pagină. 
    - Dacă este un utilizator extern, asigurați-vă că invitația a fost acceptată.
    - Dacă utilizatorul există în grupul permisiuni, asigurați-vă că adresa de e-mail este corectă.
    - Dacă adresa de e-mail a utilizatorilor nu este setată aici, creați o avertizare eșantion pentru acel utilizator care forțează sincronizarea acelui cont de utilizator de profilurile de utilizator din SharePoint în această colecție de site-uri.
 
2. E-mailul de la fluxurile de lucru este trimis administratorilor colecției de site-uri, dar nu și altor utilizatori și vedeți eroarea **http interzisă <span>https:</span>//URL/_vti_bin/client.XVC.SP.Utilities.Utility.SendEmail**.
 

    Consultați [Access Denied atunci când trimiteți un mesaj de e-mail la un grup SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    De asemenea, Verificați dacă caracteristica de colecție de site-uri cu **acces limitat la permisiune utilizator** nu este activă.


## <a name="related-topics"></a>Subiecte asociate
Doriți să încercați Microsoft Flow în SharePoint Online?
- [Crearea fluxului](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


