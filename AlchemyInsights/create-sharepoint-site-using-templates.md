---
title: Crearea unui site în SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755320"
---
# <a name="create-sharepoint-sites-using-templates"></a>Crearea de site-uri SharePoint utilizând șabloane

Șabloanele de site SharePoint sunt definiții predefinite proiectate în jurul unei nevoi speciale de afaceri. Pentru mai multe informații, consultați [utilizarea șabloanelor pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Iată câteva probleme/soluții obișnuite privind salvarea unui site sau a unei liste ca șablon în SharePoint Online. 

**Salvați butonul șablon de site/listă nu este disponibil sau lipsește**

Administratorii vor trebui să permită script particularizat pentru a activa caracteristicile șablonului. Pentru pași detaliați, exemplele și considerațiile 

- [Permiteți sau împiedicați scriptul particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.

**Imposibil de creat șablonul de site sau nu funcționează corect**

Este posibil ca șablonul să lipsească o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și să nu se activeze. Dacă caracteristica nu este disponibilă pentru a activa în colecția de site-uri curentă, nu se poate utiliza șablonul de site-ul pentru a crea un site.

- Verificați pentru a vedea dacă orice liste sau biblioteci depășesc [pragul de vedere listă limită](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 elemente, deoarece acest lucru poate bloca crearea unui șablon de site-ul.

- Site-ul poate fi folosind prea multe resurse și, prin urmare, șablonul de site-ul depășește limita de 50 MB.


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați [șablon generat listă nu afișează date din Listă tabel de căutare corectă în SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Pentru informații mai detaliate despre problemele și soluțiile obișnuite, consultați [crearea și utilizarea șabloanelor de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



