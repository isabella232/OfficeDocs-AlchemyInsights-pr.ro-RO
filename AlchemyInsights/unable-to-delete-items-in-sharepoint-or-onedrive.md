---
title: Nu se pot șterge elemente din SharePoint sau OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038529"
---
# <a name="unable-to-delete-items"></a>Nu se pot șterge elemente

- Politicile de conservare pot provoca acest lucru; trebuie fie să dezactivați, fie să excludeți reținerea în așteptare care provoacă problema. După ce o politică de retenție sau o reținere este eliminată, poate dura până la 24 de ore pentru ca modificarea să aibă efect. Asigurați-vă că nu există o configurare a [politicii de retenție](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) pentru element.

- Este posibil ca site-ul să fi depășit limita de stocare, să [mărească cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.

- Asigurați-vă că elementul [nu este extras](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) pentru un alt utilizator.

- În sfârșit, administratorii pot utiliza [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), care conține o bibliotecă de comenzi PowerShell care vă permite să efectuați acțiuni complexe de gestionare, cum ar fi ștergerea elementelor de bază.
- [Eliminarea fișierului PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Eliminarea folderului PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Remove PNP List Item](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eliminare Listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eliminarea câmpului PNP (coloană)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)