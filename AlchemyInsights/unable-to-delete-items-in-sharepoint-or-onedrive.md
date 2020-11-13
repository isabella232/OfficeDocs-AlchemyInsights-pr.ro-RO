---
title: Nu se pot șterge elemente în SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019595"
---
# <a name="unable-to-delete-items"></a>Nu se pot șterge elemente

- Politicile de retenție pot provoca acest lucru, trebuie să dezactivați sau să excludeți respectiva fixare care cauzează această problemă. După eliminarea unei politici de retenție sau a unei rețineri, poate dura până la 24 de ore pentru ca modificarea să aibă efect. Asigurați-vă că nu există o configurare a [politicii de retenție](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pentru element.

- Este posibil ca site-ul să fi depășit limita de stocare, să mărească [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.

- Asigurați-vă că elementul nu este [extras](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) unui alt utilizator.

- În cele din urmă, administratorii pot utiliza [modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni de gestionare complexe, cum ar fi să Impuneți ștergerea elementelor încăpățânat.
- [Eliminare fișier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Eliminare folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Eliminare element listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eliminare listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eliminare câmp PNP (coloană)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)