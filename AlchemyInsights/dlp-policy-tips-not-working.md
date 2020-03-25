---
title: Dlp Politica Sfaturi nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932598"
---
# <a name="dlp-policy-tip-issues"></a>Probleme cu vârful de politică DLP

**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal. Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă. În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.

În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii. Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade. Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.

**Sfaturi de politică DLP**

Când se **utilizează politici DLP**, utilizatorii pot fi notificați cu privire la o încălcare a politicii cu **sfaturi de politică**. Administratorii pot configura sfaturi de politică pentru a afișa în timp ce testează politica DLP sau atunci când politica este în modul de aplicare completă.
  
Pentru a configura sfaturi de politică privind politica DLP în centrul de securitate și conformitate în modul de aplicare completă, procedați astfel:
  
- Asigurați-vă că sfaturile de **politică** au fost activate pe regula DLP utilizând pașii [de aici](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Asigurați-vă că **conținutul corespunde cu** ceea ce este **necesar** pentru a declanșa regula descrisă în acest articol [aici](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Sfaturi de politică se afișează atât în OWA, cât și în Outlook. Cu toate acestea, atunci când se utilizează **Outlook 2013 sau o versiune ulterioară**, sfaturi de politică sunt afișate numai în anumite condiții. Aceste condiții sunt listate aici: [condiții acceptate pentru Outlook 2013 sau o versiune ulterioară pentru afișarea sfaturilor de politică](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Pentru informații suplimentare despre sfaturile de politică DLP, consultați: [Afișare sfaturi de politică pentru politicile DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  