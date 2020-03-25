---
title: DLP poate avea nevoie de un tip particularizat
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932670"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP poate avea nevoie de un tip particularizat

**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal. Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă. În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.

În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii. Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade. Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.

**DLP poate necesita un tip de informații particularizat**

Cu o politică de prevenire a pierderilor de date (DLP), puteți identifica și proteja datele sensibile din organizația dvs. În unele scenarii, poate fi necesar să creați propriul tip de informații sensibile **particularizate** pentru a proteja datele organizației.

De exemplu, este posibil ca organizația să trebuiască să identifice și să protejeze ID-urile angajaților sau alte date într-un format specific orgului dvs. Dacă da, consultați următoarele articole pentru mai multe informații.
  
 **Particularizarea unui tip de informații sensibile încorporate**
  
Dacă un tip de informații sensibile încorporat ar satisface nevoile dvs., cu doar câteva trucuri, puteți [personaliza un tip de informații sensibile încorporat](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). De exemplu, aveți posibilitatea să adăugați sau să eliminați cuvinte cheie sau să adăugați sau să eliminați dovezi justificative, ar fi o dată sau o adresă.
  
 **Crearea unui tip de informații sensibile particularizate**
  
Dar dacă trebuie să identificați și să protejați cu totul un alt tip de informații sensibile, puteți [crea un tip de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) în interfața cu utilizatorul a Centrului de securitate & conformitate.
  
**Crearea unui tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell**

În cele din urmă, dacă interfața cu utilizatorul nu furnizează toate opțiunile de care aveți nevoie, aveți posibilitatea să [creați un tip de informații sensibile particularizate în Security & Centrul de conformitate PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Începând cu un fișier XML, aveți posibilitatea să utilizați toate opțiunile disponibile.
