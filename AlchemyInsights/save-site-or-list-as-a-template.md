---
title: Salvare site sau listă ca șablon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048736"
---
# <a name="save-site-or-list-as-a-template"></a>Salvare site sau listă ca șablon

Șabloanele de site SharePoint sunt definiții predefinite proiectate în jurul unei nevoi speciale de afaceri. Pentru mai multe informații, consultați [utilizarea șabloanelor pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Iată câteva probleme/soluții obișnuite privind salvarea unui site sau a unei liste ca șablon în SharePoint Online.

**Salvați butonul șablon de site/listă nu este disponibil sau lipsește**. 

- Administratorii vor trebui să permită script particularizat pentru a activa caracteristicile șablonului. Pentru pași detaliați, exemple și considerații vedeți [Permiteți sau împiedicați scriptul particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.


**Imposibil de creat șablonul de site sau nu funcționează corect**

- Este posibil ca șablonul să lipsească o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și să nu se activeze. Dacă caracteristica nu este disponibilă pentru a activa în colecția de site-uri curentă, nu se poate utiliza șablonul de site-ul pentru a crea un site.


- Verificați pentru a vedea dacă orice liste sau biblioteci depășesc [pragul de vedere listă limită](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 elemente, deoarece acest lucru poate bloca crearea unui șablon de site-ul.


- Site-ul poate utiliza prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 megaocteți (MO).


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați [șablon generat listă nu afișează date din Listă tabel de căutare corectă în SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Pentru informații mai detaliate despre problemele și soluțiile obișnuite, vă rugăm să consultați, să [Creați și să utilizați șabloane de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

