---
title: Salvare listă sau site-ul ca un şablon
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551643"
---
# <a name="save-site-or-list-as-a-template"></a>Salvare listă sau site-ul ca un şablon

Șabloanele de site SharePoint sunt precompilate definiţii concepute în jurul o afacere special nevoie. Pentru informaţii suplimentare, consultaţi [utilizarea template-uri pentru a crea diferite tipuri de site-uri SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Aici sunt unele probleme/solutii comune cu privire la salvarea un site-ul sau lista ca şablon în SharePoint Online.

**Salvaţi site/listă şablon buton este nu folositor sau lipsă**. 

- Administratorii va trebui să permite script-ul personalizat pentru a activa caracteristicile şablon. Pentru măsurile detaliate, exemple şi consideraţii [permite sau împiedică script-ul personalizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Site-ul salvaţi ca şablon de comandă nu este acceptată şi pot provoca probleme de pe site-urile care folosesc infrastructura de publicare SharePoint Server.


**Șablonul de site-ul nu poate fi creat sau nu funcţionează corect**

- Poate să lipsească o [caracteristica](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) si nu se va activa. Dacă funcţia nu este disponibilă pentru a activa în colecția de site-ul curent, se poate utiliza site-ul şablon pentru a crea un site.


- Verificaţi pentru a vedea dacă orice liste sau biblioteci depăşi [Prag limită de vizualizare listă](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 de articole ca acest lucru poate bloca crearea unui şablon de site-ul.


- Site-ul poate folosi prea multe resurse si, prin urmare, site-ul şablon depășește limita de 50 megabyte (MB).


- Există probleme afişarea datelor dintr-o listă care utilizează o coloană de căutare. Pentru informaţii suplimentare, consultaţi [generat şablon listă nu afişează datele din lista de căutare corectă în SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Pentru informaţii mai detaliate pe probleme comune şi soluţii, vă rugăm să referinţă, [crearea şi utilizarea site-ul template-uri](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

