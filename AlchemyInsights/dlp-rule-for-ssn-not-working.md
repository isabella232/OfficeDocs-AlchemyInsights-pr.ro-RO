---
title: DlP regulă pentru SSN nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977318"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP probleme cu numerele de securitate socială

**Important:** În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile - vizitați [Ajustări le caracteristică temporară SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**DlP probleme cu SSNs**

Aveți probleme cu **data loss Prevention (DLP)** nu funcționează pentru conținut care conține un număr de securitate **socială (SSN)** atunci când utilizați un tip de informații sensibile în Office 365? Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP. 
  
De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat

- **[Model de model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSN-uri în patru modele diferite:

  - Func_ssn găsește SSN-uri cu formatare puternică pre-2011 care sunt formatate cu linițe sau spații (ddd-dddd SAU ddd ddd dddd)

  - Func_unformatted_ssn găsește SSN-uri cu formatare puternică pre-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)

  - Func_randomized_formatted_ssn găsește SSN-urile post-2011 care sunt formatate cu linițe sau spații (ddd-dd-dddd SAU ddd ddd dddd)

  - Func_randomized_unformatted_ssn găsește SSN-urile post-2011 care nu sunt formatate ca nouă cifre consecutive (dddddddddd)

- **[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nu, nu există nici un Checksum

- **[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** O politică DLP este 85% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:

  - [Funcția Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) găsește conținut care se potrivește cu modelul.

  - Se găsește un cuvânt cheie din [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Exemple de cuvinte cheie includ: *Securitate socială, Securitate Socială#, Soc Sec ,SSN* . De exemplu, următorul eșantion ar declanșa pentru politica DLP SSN: **SSN: 489-36-8350**
  
Pentru mai multe informații despre ceea ce este necesar pentru ssn-uri pentru a fi detectate pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce tipuri de informații sensibile caută SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  