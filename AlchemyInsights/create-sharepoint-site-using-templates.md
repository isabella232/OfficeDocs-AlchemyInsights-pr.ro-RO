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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057978"
---
# <a name="create-sharepoint-sites-using-templates"></a>Crearea de SharePoint-uri utilizând șabloane

Capacitatea de a salva un site ca șablon nu este acceptată cu site-urile moderne de comunicare sau de echipă. Pentru mai multe informații despre utilizarea șabloanelor, consultați [Salvarea, descărcarea și încărcarea unui site SharePoint ca șablon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Iată câteva probleme/soluții obișnuite cu privire la Salvarea unui site sau a unei liste ca șablon în SharePoint Online. 

**Butonul Salvare șablon de site/listă nu este disponibil sau lipsește**

Administratorii trebuie să permită scripturile particularizate pentru a activa caracteristicile șablonului. Pentru pași detaliați, vedeți exemple și considerații 

- [Permiterea sau blocarea scripturilor particularizate](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Comanda Salvare site ca șablon nu este acceptată și poate provoca probleme pe site-urile care utilizează infrastructura de publicare SharePoint Server.

**Șablonul de site nu poate fi creat sau nu funcționează corect**

Este posibil ca șablonului să îi [lipsească o](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) caracteristică și să nu se activeze. Dacă această caracteristică nu este disponibilă pentru activare în colecția de site-uri curentă, nu puteți utiliza șablonul de site pentru a crea un site.

- Verificați dacă vreo listă sau bibliotecă depășește [Pragul limită de vizualizare listă](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 de elemente, deoarece acest lucru poate bloca crearea unui șablon de site.

- Site-ul poate utiliza prea multe resurse și, prin urmare, șablonul de site depășește limita de 50 MB.


- Există probleme la afișarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru mai multe informații, consultați [Lista generată din șablon nu afișează datele din lista de căutare corectă din SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Pentru informații mai detaliate despre problemele comune și soluții, consultați Crearea [și utilizarea șabloanelor de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



