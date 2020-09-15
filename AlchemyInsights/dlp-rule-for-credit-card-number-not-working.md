---
title: Regulă DLP pentru numărul cardului de credit nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679453"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Probleme DLP cu numerele cardului de credit

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele cardului de credit**

Aveți probleme cu **prevenirea pierderii datelor (DLP)** nu funcționează pentru conținutul care conține un **număr de card de credit** atunci când utilizați un tip de informații DLP sensibile în O365? Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluată. De exemplu, pentru o **politică a cardului de credit** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddddddddddd) și trebuie să treacă testul Luhn.

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Model foarte complex și robust care detectează cărți din toate marile branduri din întreaga lume, inclusiv Visa, MasterCard, Discover card, JCB, American Express, Gift Cards și Diner Cards.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, checksum Luhn

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** O politică DLP este 85% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcția Func_credit_card găsește conținut care se potrivește cu modelul.

  - Una dintre următoarele este True:

  - S-a găsit un cuvânt cheie din Keyword_cc_verification.

  - S-a găsit un cuvânt cheie din Keyword_cc_name

  - Funcția Func_expiration_date găsește o dată în formatul de dată potrivit.

  - Valoarea de control trece

    De exemplu, următorul eșantion ar declanșa o politică de număr a cardului de credit DLP:

  - Viză: 4485 3647 3952 7352
  
  - Expiră: 2/2009

Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de card de credit** să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile caută cardul de credit #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  