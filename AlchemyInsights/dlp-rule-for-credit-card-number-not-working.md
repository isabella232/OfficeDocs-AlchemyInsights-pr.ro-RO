---
title: Dlp Regulă pentru numărul cardului de credit nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704213"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleme cu numerele de card de credit

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**DLP probleme cu numerele de card de credit**

Aveți probleme cu **prevenirea pierderilor de date (DLP)** nu funcționează pentru conținut care conține un **număr de card de credit** atunci când utilizați un tip de informații sensibile DLP în O365? Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluat. De exemplu, pentru o **politică de card de credit** configurat cu un nivel de încredere de 85%, următoarele sunt evaluate și trebuie să fie detectate pentru regula pentru a declanșa:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddddddddd) și trebuie să treacă testul Luhn.

- **[Model de model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Model foarte complex și robust, care detectează carduri de la toate mărcile importante din întreaga lume, inclusiv Visa, MasterCard, Discover Card, JCB, American Express, carduri cadou și carduri de restaurant.

- **[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, suma de control Luhn

- **[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:

  - Funcția Func_credit_card găsește conținut care se potrivește cu modelul.

  - Una dintre următoarele este adevărat:

  - Se găsește un cuvânt cheie din Keyword_cc_verification.

  - Se găsește un cuvânt cheie din Keyword_cc_name

  - Funcția Func_expiration_date găsește o dată în formatul de dată corect.

  - Suma de control trece

    De exemplu, următorul eșantion ar declanșa pentru o politică de număr dlp card de credit:

  - Viza: 4485 3647 3952 7352
  
  - Expiră: 2/2009

Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de card de credit** să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: Ce caută tipurile de informații [sensibile pentru cardul de credit#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  