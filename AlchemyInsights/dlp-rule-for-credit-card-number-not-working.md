---
title: Dlp Regulă pentru numărul cardului de credit nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977210"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP probleme cu numerele de card de credit

**Important:** În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile - vizitați [Ajustări le caracteristică temporară SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

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
  