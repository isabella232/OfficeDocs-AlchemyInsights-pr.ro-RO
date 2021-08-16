---
title: Regulă DLP pentru că numărul pașaportului din SUA/Regatul Unit nu funcționează
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004958"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme cu numerele de pașaport DLP - SUA/Regatul Unit

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele de pașaport din SUA/Regatul Unit**

Aveți probleme cu Prevenirea pierderii datelor **(DLP)** care nu funcționează pentru conținutul care conține un număr de pașaport de **SUA/Regatul** Unit atunci când utilizați un tip de informații sensibile DLP în O365? În acest caz, asigurați-vă că tot conținutul conține informațiile necesare pentru a vedea ce caută politica DLP atunci când este evaluată.
  
De exemplu, pentru o politică de număr de pașaport din **SUA/Regatul** Unit configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie detectate pentru ca regula să declanșeze
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nouă cifre

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nouă cifre consecutive

- **[Verificări:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există niciun Checksum

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** O politică DLP este 75% sigură că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcția Func_usa_uk_passport găsește conținutul care se potrivește cu modelul.

  - A fost găsit un cuvânt Keyword_passport cheie din mai multe cuvinte cheie.

    De exemplu, următorul exemplu se declanșează pentru politica privind pașaportul din **SUA/Regatul** Unit: numărul pașaportului în SUA 123456789

Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Regatul Unit să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: Ce arată tipurile de informații sensibile ale numărului de pașaport în [SUA/Regatul](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) Unit
  
Utilizând un alt tip de informații sensibile, consultați următorul articol pentru informații despre ceea ce este necesar pentru alte tipuri: Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  