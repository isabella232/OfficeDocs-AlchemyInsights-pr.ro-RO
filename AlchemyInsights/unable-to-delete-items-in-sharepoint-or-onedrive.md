---
title: Imposibil de șters elemente din SharePoint sau OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366545"
---
# <a name="unable-to-delete-items"></a>Imposibil de șters elemente

Probleme ştergerea elementelor?

- Întotdeauna asiguraţi-vă că aveți [permisiunile corespunzătoare](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) pentru a șterge elementul sau au o încercare de [administrator al colecției de site-ul](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) , elimina elementul.

- Asiguraţi-vă că nu există o setare de [politică de retenție](https://docs.microsoft.com/office365/securitycompliance/retention-policies) pe element.

- Asigura elementul nu este [verificat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) de către alt utilizator.

- În cele din urmă, administratorii pot utiliza [SharePoint modele şi practici](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) care conţine o bibliotecă de PowerShell comenzi care vă permite să efectuaţi acţiuni complexe de management precum forţa Ştergerea elementelor încăpăţânat.
- [Eliminaţi fişierul PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Elimina PNP Folder](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Eliminaţi elementul de listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Elimina PNP lista](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Elimina PNP câmpului (coloanei)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)