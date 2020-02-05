---
title: Crearea unui site în SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770435"
---
# <a name="create-sharepoint-sites-using-templates"></a>Crearea site-urilor SharePoint utilizând șabloane

Capacitatea de a salva un site ca șablon nu este acceptată cu site-uri moderne de comunicare sau de echipă. Pentru mai multe informații despre utilizarea șabloanelor, consultați [Salvarea, descărcarea și încărcarea unui site SharePoint ca șablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Iată câteva probleme/soluții obișnuite în ceea ce privește salvarea unui site sau a unei liste ca șablon în Sharepoint Online. 

**Butonul Salvare șablon site/listă nu este disponibil sau lipsește**

Administratorii vor trebui să permită script personalizat pentru a activa caracteristicile șablonului. Pentru pași detaliați, exemple și considerații, a se vedea 

- [Permiterea sau prevenirea scriptului particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Comanda Salvare site-ul ca șablon nu este acceptată și poate provoca probleme pe site-uri care utilizează infrastructura de publicare SharePoint Server.

**Șablonul de site nu se poate crea sau nu funcționează corect**

Este posibil ca șablonul să lipsească o [caracteristică](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) și să nu se activeze. Dacă caracteristica nu este disponibilă pentru activare în colecția de site-uri curentă, aveți posibilitatea să utilizați șablonul de site pentru a crea un site.

- Verificați dacă listele sau bibliotecile depășesc [pragul limită](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de vizualizare listă de 5000 de elemente, deoarece acest lucru poate bloca crearea unui șablon de site.

- Site-ul poate fi folosind prea multe resurse și, prin urmare, șablonul de site-ul depășește limita de 50 MB.


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați [Lista generată de șabloane nu afișează date din lista](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)de căutare corectă din SharePoint Online .

Pentru informații mai detaliate despre problemele și soluțiile obișnuite, verificați [Creați și utilizați șabloane de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



