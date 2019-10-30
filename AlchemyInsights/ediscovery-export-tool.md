---
title: Instrumentul de export eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769315"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nu se poate instala sau executa instrumentul de export eDiscovery?

Dacă nu se poate instala sau executa Office 365 eDiscovery Export Tool pentru a descărca rezultatele căutării, verificați următoarele lucruri:
  
- Computerul pe care îl utilizați îndeplinește aceste pre-rechizite:

  - 32-sau 64-bit traducere de Ferestre 7 și tîrziu traducere

  - Microsoft .NET Framework 4,7

  - Un browser acceptat:

  - Microsoft Edge

    Sau

  - Internet Explorer 10 și versiunile ulterioare

    Alte browsere, ar fi Google Chrome și Mozilla Firefox, nu sunt acceptate.

- Organizația dumneavoastră se poate conecta la punctul final în Azure, care este ** \*. blob.Core.Windows.net** (metacaractere reprezintă un Identificator unic pentru activitatea de export).

- Sunteți atribuit rolul de export în Office 365 Security &amp; conformitatea Center. În mod implicit, acest rol este atribuit numai grupului de roluri eDiscovery Manager. Consultați [atribuirea permisiunilor eDiscovery](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Pentru mai multe informații, consultați [Exportul rezultatelor căutării de conținut](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  