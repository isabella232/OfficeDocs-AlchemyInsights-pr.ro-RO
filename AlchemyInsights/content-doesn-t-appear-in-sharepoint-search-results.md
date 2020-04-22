---
title: Conținutul nu apare în rezultatele căutării SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705673"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Conținutul nu apare în rezultatele căutării SharePoint

Urmați acești pași de depanare atunci când conținutul așteptat nu apare în rezultatele căutării:
  
1. Verificați dacă **site-ul** care conține conținutul așteptat este setat pentru a permite conținutului să apară în rezultatele căutării. Urmați pașii din [Afișare conținut pe un site în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verificați dacă **lista** sau **biblioteca** care conține conținutul așteptat este setată pentru a permite conținutul să apară în rezultatele căutării. Urmați pașii [din Afișare conținut din liste sau biblioteci în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verificați dacă pagina, documentul sau aspectul particularizat al paginii sunt publicate ca **versiune majoră.** Urmați pasul 3 în [Căutare nu returnează toate rezultatele în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verificați dacă utilizatorul are **permisiuni pentru** a vizualiza conținutul. Urmați pașii din [Înțelegerea nivelurilor de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Dacă schema de căutare a fost modificată prin adăugarea unei proprietăți gestionate noi, prin editarea unei proprietăți gestionate sau prin eliminarea unei proprietăți gestionate, atunci va fi necesară o scotocire și un reindex. **Reindexați** conținutul urmând pașii din [Solicitarea manuală de scotocire și reindexare a unui site, a unei biblioteci sau a unei liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Acest lucru poate dura un timp, așteptați 24 de ore înainte de a verifica rezultatele din nou.

Pentru mai multe informații, consultați [Activarea conținutului de pe un site pentru a putea fi căutat](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
