---
title: Căutare în SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044055"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Conținut scotocire și indexare în SharePoint Online

Conținutul trebuie scotocit și adăugat la indexul de căutare pentru ca utilizatorii să găsească ceea ce caută în SharePoint Online. Conținutul este scotocit automat pe baza unui program de scotocire predefinit (programul de scotocire nu poate fi modificat). Crawlerul preia conținut care s-a modificat de la ultima accesare cu crawlere și actualizează indexul. Pentru a asigura că conținutul este scotocit și indexul este actualizat, rețineți următoarele:

- Asigurați-vă că conținutul poate fi găsit prin [crearea de conținut site-ul de căutare](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Când ați modificat o proprietate gestionată sau când ați modificat Maparea proprietăților scotocite și gestionate, situl trebuie rescotocit înainte ca modificările să se reflecte în indexul de căutare. 

    Deoarece modificările sunt făcute în schema de căutare, și nu la site-ul real, crawlerul nu va reindexa automat site-ul. 

    Pentru mai multe informații, consultați [solicitați manual accesarea cu crawlere și reindexarea unui site, a unei biblioteci sau a unei liste](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Așteptați cel puțin 24 de ore după ce solicitați manual o accesare cu crawlere și o Reindexare completă pentru a vedea dacă întâmpinați încă o problemă. 

    Dacă au trecut mai mult de 24 de ore de la inițierea scotocire și reindex complet, vă rugăm să faceți log un caz de suport. În multe cazuri, suntem deja de lucru pe o soluție. Vă rugăm să ne acordați cel puțin 24 de ore pentru a finaliza o soluție.

> [!IMPORTANT]
> Dacă un site, document (bibliotecă), sau o listă a fost șters și încă arată în rezultatele căutării, utilizatorii ar trebui să primească o **eroare 404 fișier negăsit** atunci când încearcă să-l acceseze. Această problemă ar trebui să fie înregistrată ca un caz de sprijin pentru investigații suplimentare. 



