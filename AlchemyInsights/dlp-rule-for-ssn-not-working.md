---
title: Regula DLP pentru SSN nu funcționează
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004994"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Probleme DLP cu numerele de securitate socială

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu SSN**

Aveți probleme cu Prevenirea **pierderii datelor (DLP)** care nu funcționează pentru conținut care conține un **SSN atunci** când utilizați un tip de informații sensibile în Microsoft 365? În acest caz, asigurați-vă că acest conținut conține informațiile necesare pentru a vedea ce caută politica DLP. 
  
De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie detectate pentru ca regula să se declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat

- **[Model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSN-uri în patru modele diferite:

  - Func_ssn găsește SSN cu o formatare puternică, pre-2011, care sunt formatate cu linii întrerupte sau spații (ddd-ddd-dddd OR ddd dddd)

  - Func_unformatted_ssn găsește SSN cu o formatare puternică, pre-2011, care sunt neformatate ca nouă cifre consecutive (ddddddddd)

  - Func_randomized_formatted_ssn găsește SSN-urile post-2011 care sunt formatate cu liniuțe sau spații (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn găsește SSN-urile post-2011 care sunt neformatate ca nouă cifre consecutive (ddddddddd)

- **[Verificări:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nu, nu există niciun Checksum

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** O politică DLP este 85% sigură că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcția [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) găsește conținut care se potrivește cu modelul.

  - A fost găsit un [cuvânt Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) cheie din mai multe cuvinte cheie. Exemplele de cuvinte cheie includ:  *Securitate socială, Securitate socială#, Soc Sec, SSN*  . De exemplu, următorul exemplu se declanșează pentru politica DLP SSN: **SSN: 489-36-8350**
  
Pentru mai multe informații despre ceea ce este necesar pentru ca SSN să fie detectat pentru conținut, consultați secțiunea următoare din acest articol: Ce aspect caută tipurile de informații sensibile pentru [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizând un alt tip de informații sensibile, consultați următorul articol pentru informații despre ceea ce este necesar pentru alte tipuri: Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  