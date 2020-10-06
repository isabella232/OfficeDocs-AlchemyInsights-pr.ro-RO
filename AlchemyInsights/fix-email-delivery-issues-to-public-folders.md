---
title: Remedierea problemelor de livrare a mesajelor de e-mail în folderele publice activate pentru e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366476"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Remedierea problemelor de livrare a mesajelor de e-mail în folderele publice activate pentru e-mail

Dacă expeditorii externi nu pot trimite mesaje în folderele publice activate pentru e-mail, iar expeditorii primesc eroarea: **nu s-a găsit (550 5.4.1)**, Verificați dacă domeniul de e-mail pentru folderul public este configurat ca domeniu de retransmisie internă în locul unui domeniu autoritar:

1. Deschideți [Centrul de administrare Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Accesați domeniile acceptate pentru **flux de corespondență** \> **Accepted domains**, selectați domeniul acceptat, apoi faceți clic pe **Editare**.

3. În pagina proprietăți care se deschide, dacă tipul de domeniu este setat la **autoritate**, modificați valoarea la **retransmisie internă** , apoi faceți clic pe **Salvare**.

Dacă expeditorii externi primesc eroarea pe **care nu aveți permisiunea (550 5.7.13)**, derulează următoarea comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi din folderul public:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Pentru a permite utilizatorilor externi să trimită mesaje de e-mail în acest folder public, adăugați direct CreateItems la utilizator Anonymous. De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
