---
title: Regulă DLP pentru ca Numărul de cont bancar din SUA să nu funcționează
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005030"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Probleme DLP cu numerele de cont bancar din SUA

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele de cont bancar din SUA**

Aveți probleme cu Prevenirea pierderii datelor **(DLP)** care nu funcționează pentru conținutul care conține un număr de cont bancar din **SUA** atunci când utilizați un tip de informații sensibile DLP în O365? În acest caz, asigurați-vă că tot conținutul conține informațiile necesare pentru a vedea ce caută politica DLP atunci când este evaluată.
  
De exemplu, pentru o politică de număr de cont bancar din **SUA** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 cifre consecutive.

- **[Verificări:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există niciun Checksum

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** O politică DLP este 75% sigură că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Expresia obișnuită Regex_usa_bank_account_number găsește conținut care se potrivește cu modelul

  - A fost găsit un cuvânt Keyword_usa_Bank_Account cheie din mai multe cuvinte cheie.

    De exemplu, următorul exemplu se declanșează pentru politica SUA privind numărul **de cont bancar:** Verificarea conturilor 78344011

Pentru mai multe informații despre ce este necesar pentru ca un număr de cont bancar din **SUA** să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: Ce arată tipurile de informații sensibile pentru Numărul de cont bancar din [SUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Utilizând un alt tip de informații sensibile, consultați următorul articol pentru informații despre ceea ce este necesar pentru alte tipuri: Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  