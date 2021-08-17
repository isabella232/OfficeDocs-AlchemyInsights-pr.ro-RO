---
title: Salvarea site-ului sau a listei ca șablon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109216"
---
# <a name="save-site-or-list-as-a-template"></a>Salvarea site-ului sau a listei ca șablon

SharePoint de site sunt definiții predefinite proiectate în jurul unei anumite nevoie de afaceri. Pentru mai multe informații, consultați [Utilizarea șabloanelor pentru a crea diferite tipuri de SharePoint-uri.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Iată câteva probleme/soluții obișnuite cu privire la Salvarea unui site sau a unei liste ca șablon în SharePoint Online.

**Butonul Salvare șablon de site/listă nu este disponibil sau lipsește.** 

- Administratorii trebuie să permită scripturile particularizate pentru a activa caracteristicile șablonului. Pentru pași detaliați, exemple și considerații, consultați [Permiterea sau prevenirea scriptului particularizat.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-urile care utilizează infrastructura de publicare SharePoint Server.


**Șablonul de site nu poate fi creat sau nu funcționează corect**

- Este posibil ca șablonului să îi [lipsească o](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) caracteristică și să nu se activeze. Dacă această caracteristică nu este disponibilă pentru activare în colecția de site-uri curentă, nu puteți utiliza șablonul de site pentru a crea un site.


- Verificați dacă vreo listă sau bibliotecă depășește [Pragul limită de vizualizare listă](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 de elemente, deoarece acest lucru poate bloca crearea unui șablon de site.


- Site-ul poate utiliza prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 megabaiți (MB).


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați Lista generată de la șablon nu afișează date din [lista de căutare corectă în SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Pentru mai multe informații detaliate despre problemele comune și soluții, consultați Crearea [și utilizarea șabloanelor de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

