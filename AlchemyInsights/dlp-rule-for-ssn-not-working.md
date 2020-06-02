---
title: DlP regulă pentru SSN nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507382"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP probleme cu numerele de securitate socială

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**DlP probleme cu SSNs**

Aveți probleme cu **data loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de securitate **socială (SSN)** atunci când utilizați un tip de informații sensibile în Microsoft 365? Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP. 
  
De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat

- **[Model de model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSN-uri în patru modele diferite:

  - Func_ssn găsește SSN-uri cu formatare puternică pre-2011 care sunt formatate cu linițe sau spații (ddd-dddd SAU ddd ddd dddd)

  - Func_unformatted_ssn găsește SSN-uri cu formatare puternică pre-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)

  - Func_randomized_formatted_ssn găsește SSN-urile post-2011 care sunt formatate cu linițe sau spații (ddd-dd-dddd SAU ddd ddd dddd)

  - Func_randomized_unformatted_ssn găsește SSN-urile post-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)

- **[Suma de control:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nu, nu există nici un Checksum

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:

  - [Funcția Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) găsește conținut care se potrivește cu modelul.

  - Se găsește un cuvânt cheie din [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Exemple de cuvinte cheie includ: *Securitate socială, Securitate Socială#, Soc Sec ,SSN* . De exemplu, următorul eșantion ar declanșa pentru politica DLP SSN: **SSN: 489-36-8350**
  
Pentru mai multe informații despre ceea ce este necesar pentru ssn-uri pentru a fi detectate pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce tipuri de informații sensibile caută SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  