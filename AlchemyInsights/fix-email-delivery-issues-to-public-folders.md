---
title: Remedierea problemelor de livrare a e-mailurilor în folderele publice activate pentru e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716364"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Remedierea problemelor de livrare a e-mailurilor în folderele publice activate pentru e-mail

Dacă expeditorii externi nu pot trimite mesaje către folderele publice activate pentru e-mail, iar expeditorii primesc eroarea: **nu s-a găsit (550 5.4.1),** verificați că domeniul de poștă electronică pentru folderul public este configurat ca domeniu intern de retransmisie în locul unui domeniu cu autoritate:

1. Deschideți centrul de [administrare Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Accesați **Flux de** \> **corespondență Domenii acceptate**, selectați domeniul acceptat, apoi faceți clic pe **Editare**.

3. În pagina de proprietăți care se deschide, dacă tipul de domeniu este setat la **Autoritate**, modificați valoarea la **Releu intern,** apoi faceți clic pe **Salvare**.

Dacă expeditorii externi primesc eroarea **nu aveți permisiunea (550 5.7.13),** executați următoarea comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi în folderul public:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Pentru a permite utilizatorilor externi să trimită e-mailuri în acest folder public, adăugați dreptul de acces CreateItems la utilizatorul Anonim. De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
