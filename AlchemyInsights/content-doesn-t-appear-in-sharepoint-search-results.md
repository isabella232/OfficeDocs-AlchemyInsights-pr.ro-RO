---
title: Conținutul nu apare în rezultatele căutării SharePoint
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713142"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Conținutul nu apare în rezultatele căutării SharePoint

Urmați acești pași de depanare atunci când conținutul așteptat nu apare în rezultatele căutării:
  
1. Verificați dacă **site-ul** care conține conținutul așteptat este setat pentru a permite ca conținutul să apară în rezultatele căutării. Urmați pașii din [Afișare conținut de pe un site în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Verificați dacă **lista** sau **biblioteca** care conține conținutul așteptat este setată pentru a permite ca conținutul să apară în rezultatele căutării. Urmați pașii din [Afișați conținut din liste sau biblioteci în rezultatele căutării](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Verificați dacă aspectul paginii, al documentului sau al paginii particularizate este publicat ca **versiune majoră.** Urmărirea pasul 3 din [Căutare nu returnează toate rezultatele în SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Verificați dacă utilizatorul are **permisiuni** pentru a vizualiza conținutul. Urmați pașii din [înțelegerea nivelurilor de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Dacă schema de căutare a fost modificată prin adăugarea unei noi proprietăți gestionate, prin editarea unei proprietăți gestionate sau prin eliminarea unei proprietăți gestionate, atunci solicitarea unei scotociri și Reindexare va fi necesară. **Reindexați** conținutul urmând pașii din [solicitarea manuală a accesării cu crawlere și reindexarea unui site, a unei biblioteci sau a unei liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Acest lucru poate dura un timp, așteptați 24 de ore înainte de a verifica rezultatele din nou.

Pentru mai multe informații, consultați [Activarea conținutului de pe un site pentru a fi căutat](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
