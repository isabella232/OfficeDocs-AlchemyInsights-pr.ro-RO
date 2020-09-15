---
title: Regulă DLP pentru SSN nu funcționează
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679381"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Probleme DLP cu numerele de securitate socială

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu SSNs**

Întâmpinați probleme cu **prevenirea pierderii datelor (DLP)** care nu funcționează pentru conținutul care conține un **număr de securitate socială (SSN)** atunci când utilizați un tip de informații sensibile în Microsoft 365? Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP. 
  
De exemplu, pentru o politică SSN configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, care pot fi într-un model formatat sau neformatat

- **[Model:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Patru funcții caută SSNs în patru modele diferite:

  - Func_ssn găsește SSNs cu o formatare puternică pre-2011, care este formatată cu linii întrerupte sau spații (ddd-dd-dddd sau ddd dd dddd)

  - Func_unformatted_ssn găsește SSNs cu o formatare puternică pre-2011, care este neformatată ca nouă cifre consecutive (gales)

  - Func_randomized_formatted_ssn găsește SSNs post-2011 care sunt formatate cu linii întrerupte sau spații (ddd-dd-dddd sau ddd dd dddd)

  - Func_randomized_unformatted_ssn găsește SSNs post-2011 care sunt neformatate ca nouă cifre consecutive (gales)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nu, nu există nicio sumă de control

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** O politică DLP este 85% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - [Funcția Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) găsește conținut care se potrivește cu modelul.

  - S-a găsit un cuvânt cheie din [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Exemple de cuvinte cheie includ:  *securitate socială, securitate socială #, soc sec, SSN*  . De exemplu, următorul eșantion ar declanșa politica DLP SSN: **SSN: 489-36-8350**
  
Pentru mai multe informații despre ceea ce este necesar pentru ca SSNs să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce caută tipurile de informații sensibile pentru SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  