---
title: Crearea unui site în SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732248"
---
# <a name="create-sharepoint-sites-using-templates"></a>Crearea de site-uri SharePoint utilizând șabloane

Capacitatea de a salva un site ca șablon nu este acceptată cu comunicațiile moderne sau cu site-urile de echipă. Pentru mai multe informații despre utilizarea șabloanelor [, consultați Salvarea, descărcarea și încărcarea unui site SharePoint ca șablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Iată câteva probleme comune/soluții cu privire la salvarea unui site sau a unei liste ca șablon în SharePoint Online. 

**Butonul Salvare șablon de site/listă nu este disponibil sau lipsește**

Administratorii vor trebui să permită un script particularizat pentru a activa caracteristicile șablonului. Pentru pași detaliați, exemple și considerații, consultați 

- [Permiterea sau prevenirea scripturilor particularizate](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.

**Șablonul de site nu poate fi creat sau nu funcționează corect**

Șablonul poate fi lipsește o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și nu se va activa. Dacă caracteristica nu este disponibilă pentru a fi activată în colecția de site-uri curentă, nu puteți utiliza șablonul de site pentru a crea un site.

- Verificați dacă listele sau bibliotecile depășesc [pragul limită de vizualizare a listei](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de elemente 5000, deoarece acest lucru poate bloca crearea unui șablon de site.

- Este posibil ca site-ul să utilizeze prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 MB.


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați [lista generate de șabloane nu afișează date din lista de căutare corectă din SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Pentru mai multe informații detaliate despre problemele și soluțiile comune, consultați [crearea și utilizarea șabloanelor de site](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



