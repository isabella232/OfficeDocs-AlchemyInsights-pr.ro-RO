---
title: Limitare SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931238"
---
# <a name="sharepoint-online-throttling"></a>Limitare SharePoint Online

**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal. Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă. În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.

În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii. Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade. Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.

**503 server este ocupat de eroare**

Utilizatorii pot primi un server 503 este ocupat eroare atunci când încercați să navigați la site-uri SharePoint sau OneDrive. 

Această eroare poate fi cauzată de limitare în cadrul serviciului SharePoint. SharePoint Online utilizează limitarea pentru a menține performanța optimă și fiabilitatea serviciului SharePoint Online. Limitarea limitează numărul de acțiuni ale utilizatorilor sau apeluri simultane (după script sau cod) pentru a preveni utilizarea exagerată a resurselor. 

Pentru mai multe informații despre limitare, [consultați, Evitați să fiți sugrumat sau blocat în SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Dacă credeți că această eroare nu are legătură cu limitarea, aveți posibilitatea să verificați dacă există întreținere activă care are loc pe entitategăzduită navigând la [centrul de mesaje](https://portal.office.com/adminportal/home#/MessageCenter).

 În cele din urmă, asigurați-vă că vizitați pagina [De sănătate a serviciilor](https://portal.office.com/adminportal/home#/servicehealth) pentru a verifica orice recomandări/incidente care pot apărea.

