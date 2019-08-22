---
title: Căutare în SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507643"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Accesarea cu crawlere conţinut şi indexarea în SharePoint Online

Conţinutul trebuie să fie indexat şi adăugate la indexul de căutare pentru utilizatorilor să găsească ceea ce ei caută în SharePoint Online. Conţinutul este scotocit automat bazat pe un program de accesare cu crawlere pre-definite (programul de scotocire nu poate fi schimbat). Crawler-ul preia conţinutul pe care s-a schimbat ultima scotocire şi actualizează indexul. Pentru a se asigura de conţinut este indexat şi Indexul este actualizat, reţineţi următoarele:

- Asiguraţi-vă că de conţinut pot fi găsite făcând [conţinutul site-ului poate fi căutat](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Aţi modificat o proprietate gestionată, sau atunci când aţi schimbat cartografierea accesate şi gestionate proprietăţi, site-ul trebuie să fie re-scotocite înainte de modificările vor fi reflectate în indexul de căutare. 

    Deoarece modificările sunt făcute în schemă de căutare, şi nu la site-ul real, crawlerul va automat re-indexa site-ul. 

    Pentru mai multe informaţii, consultaţi [manual solicita accesarea cu crawlere şi re-indexarea unui site, o listă sau o bibliotecă](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Aşteptaţi cel puţin 24 de ore după manual solicită o accesare cu crawlere şi complet re-index pentru a vedea dacă vă confruntaţi în continuare o problemă. 

    În cazul în care mai mult de 24 de ore au trecut de cand ai initiat de accesare cu crawlere şi complet re-indexa, vă rugăm să vă un caz de suport. În multe cazuri, lucrăm deja la o soluţie. Vă rugăm să ne dea cel puţin 24 de ore pentru a finaliza o soluţie.

> [!IMPORTANT]
> În cazul în care un site, documentul (biblioteca), sau o listă a fost şters şi prezintă încă în rezultatele de căutare, utilizatorii ar trebui să primiţi o **Eroare 404 Fişier negăsit** atunci când încearcă să-l acces. Această problemă trebuie să fiţi conectat ca un caz de suport pentru o analiza ulterioara. 



