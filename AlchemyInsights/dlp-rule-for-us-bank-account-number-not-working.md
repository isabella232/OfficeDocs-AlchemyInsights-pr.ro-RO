---
title: Regulă DLP pentru numărul de cont bancar din S.U.A. nu funcționează
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679308"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Probleme DLP cu numerele conturilor bancare din SUA

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

**Probleme DLP cu numerele conturilor bancare din SUA**

Aveți probleme cu **prevenirea pierderii datelor (DLP)** nu funcționează pentru conținutul care conține un **număr de cont bancar din s.u.a.** atunci când utilizați un tip de informații DLP sensibile în O365? Dacă este așa, asigurați-vă că conținutul conține informațiile necesare pentru ceea ce caută politica DLP atunci când este evaluată.
  
De exemplu, pentru o politică de **număr de cont bancar din s.u.a.** configurată cu un nivel de încredere de 85%, sunt evaluate următoarele și trebuie să fie detectate pentru ca regula să declanșeze:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre

- **[Model:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 cifre consecutive.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nu, nu există nicio sumă de control

- **[Definiție:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** O politică DLP este 75% încrezător că a detectat acest tip de informații sensibile dacă, într-o proximitate de 300 de caractere:

  - Expresia obișnuită Regex_usa_bank_account_number găsește conținut care se potrivește cu modelul

  - S-a găsit un cuvânt cheie din Keyword_usa_Bank_Account.

    De exemplu, următorul eșantion ar declanșa Politica de **număr al contului bancar din SUA** : verificarea contului 78344011

Pentru mai multe informații despre ceea ce este necesar pentru ca un **număr de cont bancar din s.u.a.** să fie detectat pentru conținutul dvs., consultați secțiunea următoare din acest articol: [ce tipuri de informații sensibile ne caută numărul de cont bancar din SUA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Utilizând un alt tip de informații sensibile predefinite, consultați următorul articol pentru informații despre ce este necesar pentru alte tipuri: [ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  