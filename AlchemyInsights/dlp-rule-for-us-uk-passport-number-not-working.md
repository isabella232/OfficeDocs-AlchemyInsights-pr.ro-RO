---
title: DlP regulă pentru SUA / Marea Britanie Pașaport Numărul nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507310"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme cu DLP - SUA / Marea Britanie numerede pașaport

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**DLP probleme cu SUA / Marea Britanie numerede pașaport**

Aveți probleme cu **prevenirea pierderilor de date (DLP)** care nu funcționează pentru conținut care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații sensibile DLP în O365? Dacă da, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce politica DLP caută atunci când este evaluat.
  
De exemplu, pentru o politică **de număr de pașaport SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nouă cifre

- **[Model de model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nouă cifre consecutive

- **[Suma de control:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nici un Checksum

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** O politică DLP este 75% încrezător că este detectat acest tip de informații sensibile în cazul în care, într-o apropiere de 300 de caractere:

  - Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.

  - Se găsește un cuvânt cheie din Keyword_passport.

    De exemplu, următorul eșantion ar declanșa politica **privind numărul pașaportului SUA/Regatul Unit:** numărul pașaportului SUA 123456789

Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Marea Britanie să fie detectat pentru conținutul dvs., consultați următoarea secțiune din acest articol: [Ce caută tipurile de informații sensibile pentru numărul pașaportului SUA/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Utilizând un alt tip de informații sensibile încorporat, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  