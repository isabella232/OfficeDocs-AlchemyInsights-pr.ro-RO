---
title: Flux de lucru e-mail nu este trimis
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059615"
---
# <a name="workflow-email-is-not-being-sent"></a>Flux de lucru e-mail nu este trimis

1. E-mail de la fluxurile de lucru nu sunt trimise tuturor utilizatorilor sau doar anumiţi utilizatori, sau tu a vedea eroare **mesajul de poștă electronică nu poate fi trimis. Asiguraţi-vă că adresa de e-mail a destinatarului valid**.

Verificaţi dacă utilizatorul există în **Toţi oamenii** permisiunile grupului (lista informații utilizator) pentru că colecției de site-uri.  Proba directă URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- În cazul în care utilizatorul nu exista, asiguraţi-vă că utilizatorul este semnat în pagină. 
- În cazul în care este un utilizator extern, asiguraţi-vă că invitaţia a fost acceptată.
- Dacă utilizatorul există în grupul de permisiuni, asiguraţi-vă că adresa de e-mail este corectă.
- În cazul în care adresa de e-mail a utilizatorilor nu este stabilit aici, apoi creaţi o alertă de probă pentru acel utilizator care forţele sincronizare acel cont de utilizator la User profile de SharePoint pentru această colecție de site-ul.
 
2. E-mail de la fluxuri de lucru sunt trimise la administratori ai colecției de site-ul dar nu de la alţi utilizatori şi vedea de eroare **HTTP interzis să <spam> <spam> ** <spam> <spam>.
 

A se vedea [Acces refuzat atunci când grupuri de poştă electronică să](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

De asemenea, să verifice dacă caracteristica de colectare **modul acces limitat utilizator permisiunea lockdown** site-ul nu este activ.

## <a name="related-topics"></a>Subiecte asociate
- [Crea fluxul](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint şi fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


