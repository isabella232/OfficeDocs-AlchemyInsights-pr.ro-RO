---
title: Imposibil de șters elemente din SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571283"
---
# <a name="unable-to-delete-items"></a>Imposibil de șters elementele

Politicile de retenție pot provoca acest lucru, trebuie să dezactivați sau să excludeți reținerea respectivă care cauzează această problemă. După ce o politică de retenție sau reținerea este eliminată, poate dura până la 24 de ore pentru ca modificarea să aibă efect. Asigurați-vă că nu există o configurare [de politică](https://docs.microsoft.com/office365/securitycompliance/retention-policies) de conservare pe elementul.

Este posibil ca site-ul să fi depășit limita de stocare, să crească [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.

Asigurați-vă că elementul nu este [extras](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) către un alt utilizator.

În cele din urmă, administratorii pot utiliza [Modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni complexe de gestionare, ar fi ștergerea forțată elemente încăpățânat.
- [Eliminare fișier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Eliminare folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Eliminare element listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eliminare listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eliminare câmp PNP (coloană)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)