---
title: Imposibil de șters elementele din SharePoint sau OneDrive
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511988"
---
# <a name="unable-to-delete-items"></a>Imposibil de șters elemente

Politicile de conservare poate provoca acest lucru, trebuie să dezactivați sau exclude țirea respectivă care cauzează această problemă. După ce o politică de conservare sau de așteptare este eliminat, poate dura până la 24 de ore pentru ca modificarea să intre în vigoare. Asigurați-vă că nu există o [configurare a politicii](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) de conservare pe element.

Este posibil ca site-ul să fi depășit limita de stocare, să mărească [cota de site](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) și să șteargă elementul.

Asigurați-vă că elementul nu este [extras la](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) un alt utilizator.

În cele din urmă, administratorii pot utiliza [Modele și practici SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) care conține o bibliotecă de comenzi PowerShell care vă permit să efectuați acțiuni complexe de gestionare, ar fi eliminarea forțată elemente încăpățânate.
- [Eliminare fișier PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Eliminare folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Eliminare element listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eliminare listă PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eliminare câmp PNP (coloană)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)