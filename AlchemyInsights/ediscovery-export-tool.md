---
title: Instrumentul de export pentru descoperirea informațiilor electronic
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101314"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nu puteți să instalați sau să rulați Instrumentul de export pentru descoperirea informațiilor electronic?

Dacă nu puteți instala sau rula Instrumentul de export pentru descoperirea informațiilor electronic pentru a descărca rezultatele căutării, verificați următoarele:
  
- Computerul pe care îl utilizați îndeplinește aceste cerințe predefinite:

  - Versiuni pe 32 sau pe 64 de biți de Windows 7 și versiuni mai recente

  - Microsoft .NET Framework 4.7

  - Un browser acceptat:

  - Microsoft Edge

    Sau

  - Internet Explorer 10 și versiuni mai recente

    Alte browsere, cum ar fi Google Chrome și Mozilla Firefox nu sunt acceptate.

- Organizația dvs. se poate conecta la punctul final în Azure, care este **\* .blob.core.windows.net** (wildcardul reprezintă un identificator unic pentru munca dvs. de export).

- I s-a atribuit rolul Export în Centrul de conformitate Microsoft 365 &amp; securitate. În mod implicit, acest rol este atribuit doar grupului de roluri Manager pentru descoperirea informațiilor electronic. Consultați [Atribuirea permisiunilor de descoperire a informațiilor electronic.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Pentru mai multe informații, consultați [Exportul rezultatelor căutării de conținut.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Dacă exportați mai mult de 100.000 de cutii poștale, va trebui să utilizați următorul Powershell pentru a descărca rezultatele exportului: exportul rezultatelor din peste  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)de cutii poștale.