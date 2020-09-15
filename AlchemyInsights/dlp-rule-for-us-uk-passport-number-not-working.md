---
title: Regulă DLP pentru numărul de pașaport pentru SUA/Regatul Unit nu funcționează
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679236"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme cu numerele de pașaport DLP-US/UK

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele de pașaport din SUA/Marea Britanie**

Întâmpinați probleme cu **prevenirea pierderii datelor (DLP)** care nu funcționează pentru conținutul care conține un **număr de pașaport SUA/Marea Britanie** atunci când utilizați un tip de informații DLP sensibile în O365? Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP atunci când este evaluată.
  
De exemplu, pentru o politică de **număr pașaport din SUA/Marea Britanie** configurată cu un nivel de încredere de 75%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să fie declanșată
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nouă cifre

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nouă cifre consecutive

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nicio sumă de control

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** O politică DLP este 75% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Funcția Func_usa_uk_passport găsește conținut care se potrivește cu modelul.

  - S-a găsit un cuvânt cheie din Keyword_passport.

    De exemplu, următorul eșantion ar declanșa politica pentru **numărul de pașapoarte din SUA/Marea Britanie** : pașaportul s.u.a. numărul 123456789

Pentru mai multe informații despre ceea ce este necesar pentru ca un număr de pașaport din SUA/Regatul Unit să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile ne arată numărul de pașaport pentru SUA/Regatul Unit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  