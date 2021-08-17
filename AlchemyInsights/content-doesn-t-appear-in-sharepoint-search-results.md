---
title: Conținutul nu apare în rezultatele SharePoint căutare
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081622"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Conținutul nu apare în rezultatele SharePoint căutare

Urmați acești pași de depanare atunci când nu apare conținutul așteptat în rezultatele căutării:
  
1. Verificați dacă **site-ul** care conține conținutul așteptat este setat pentru a permite apariția conținutului în rezultatele căutării. Urmați pașii din [Afișare conținut de pe un site în rezultatele căutării.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Verificați dacă lista **sau** biblioteca **care conține** conținutul așteptat este setată să permită apariția conținutului în rezultatele căutării. Urmați pașii din [Afișarea conținutului din liste sau biblioteci în rezultatele căutării.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Verificați dacă aspectul paginii, documentului sau paginii particularizate este publicat ca **versiune Majoră.** Urmați pasul 3 [din Căutare nu returnează toate rezultatele în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verificați dacă utilizatorul are **permisiunea** de a vizualiza conținutul. Urmați pașii din [Înțelegerea nivelurilor de permisiune SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Dacă schema de căutare a fost modificată prin adăugarea unei noi proprietăți gestionate, prin editarea unei proprietăți gestionate sau prin eliminarea unei proprietăți gestionate, apoi solicitarea unei scotociri și re-indexare va fi necesară. **Re indexați** conținutul urmând pașii din Solicitarea manuală a accesatului cu crawlere și [re indexarea unui site, a](https://docs.microsoft.com/sharepoint/crawl-site-content)unei biblioteci sau a unei liste. Acest lucru poate dura un timp, așteptați 24 de ore înainte să verificați din nou rezultatele.

Pentru mai multe informații, consultați [Activarea căutării conținutului de pe un site.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
