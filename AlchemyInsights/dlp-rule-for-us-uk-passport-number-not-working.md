---
title: DlP regulă pentru SUA / Marea Britanie Pașaport Numărul nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977118"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme cu DLP - SUA / Marea Britanie numerede pașaport

**Important:** În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile - vizitați [Ajustări le caracteristică temporară SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**DLP probleme cu SUA / Marea Britanie numerede pașaport**

Aveți probleme cu **prevenirea pierderilor de date (DLP)** care nu funcționează pentru conținut care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații sensibile DLP în O365? Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.
  
De exemplu, pentru o politică **de număr de pașaport SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nouă cifre

- **[Model de model:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nouă cifre consecutive

- **[Suma de control:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nu, nu există nici un Checksum

- **[Definiție:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:

  - Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.

  - Se găsește un cuvânt cheie din Keyword_passport.

    De exemplu, următorul eșantion ar declanșa politica **privind numărul pașaportului SUA/Regatul Unit:** numărul pașaportului SUA 123456789

Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Marea Britanie să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce caută tipurile de informații sensibile pentru numărul pașaportului SUA/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  