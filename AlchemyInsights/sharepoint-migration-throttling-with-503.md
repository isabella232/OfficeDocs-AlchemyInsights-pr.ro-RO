---
title: Migrare SharePoint limitare cu 503 erori
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931670"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>Migrare SharePoint limitare cu 503 erori

**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal. Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă. În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.

În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii. Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade. Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.

**503 erori la migrarea la SharePoint Online**

Se pare că migrați la SharePoint Online și primiți 503 erori. Vă rugăm să urmați pașii de mai jos, astfel încât să vă putem ajuta cât mai curând posibil. 

1. Faceți clic pe **Contact Support**, apoi pe Solicitare **serviciu nou**.
2. Pentru titlu și descriere, tastați **Throttling migrare SharePoint cu 503**.
3. După ce biletul a fost remis, vă rugăm să îl actualizați cu următoarele informații:
    - Cât de mult a mai rămas din migrație (de exemplu, cât de multe TBs?).
    - Data de început și de sfârșit a migrării.
    - Descrieți de unde migrați conținutul, ar fi SharePoint Server, Box, GDrive, Partajări de fișiere etc..
    - Estimați numărul de erori de limitare (de exemplu, x accelerație pe oră?) și când s-a întâmplat limitarea.
    - Ce instrument de migrare utilizați (de exemplu, SPMT sau ShareGate).


