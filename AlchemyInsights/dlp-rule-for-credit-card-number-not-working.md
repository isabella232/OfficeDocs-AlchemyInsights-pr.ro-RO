---
title: Regulă DLP pentru ne funcționează numărul de card de credit
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005102"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Probleme DLP cu numerele de cărți de credit

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele de cărți de credit**

Aveți probleme cu Prevenirea pierderii datelor **(DLP)** care nu funcționează pentru conținutul care conține un număr de card de **credit** atunci când utilizați un tip de informații sensibile DLP în O365? În acest caz, asigurați-vă că tot conținutul conține informațiile necesare pentru a declanșa politica DLP atunci când este evaluată. De exemplu, pentru o politică de carte de **credit** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să se declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre care pot fi formatate sau neformatate (dddddddd) și trebuie să treacă testul Luhn.

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Model foarte complex și robust, care detectează cardurile de la toate mărcile importante din întreaga lume, inclusiv Visa, MasterCard, Discover Card, JCB, American Express, carduri cadou și carduri de restaurant.

- **[Verificări:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, verificările Iulia

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** O politică DLP este 85% sigură că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcția Func_credit_card găsește conținutul care se potrivește cu modelul.

  - Una dintre următoarele variante este adevărată:

  - A fost găsit un cuvânt Keyword_cc_verification cheie dintr-un cuvânt cheie.

  - A keyword from Keyword_cc_name is found

  - Funcția Func_expiration_date găsește o dată în formatul corect de dată.

  - Verificările sunt trecute

    De exemplu, următorul exemplu se declanșează pentru o politică de numere de carte de credit DLP:

  - Visa: 4485 3647 3952 7352
  
  - Expiră: 2/2009

Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de card de **credit** să fie detectat pentru conținut, consultați secțiunea următoare din acest articol: Ce aspect caută tipurile de informații sensibile pentru cărțile de [credit#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Utilizând un alt tip de informații sensibile, consultați următorul articol pentru informații despre ceea ce este necesar pentru alte tipuri: Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  