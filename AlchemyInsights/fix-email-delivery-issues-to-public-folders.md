---
title: Rezolva problemele de livrare e-mail la folderele publice cu corespondenţa activată
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525138"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rezolva problemele de livrare e-mail la folderele publice cu corespondenţa activată

Dacă expeditori externi nu pot trimite mesaje la folderele publice cu corespondenţa activată şi expeditorii primesc eroare: **nu a putut fi găsit (550 5.4.1)**, verificaţi dacă domeniul de e-mail pentru folderul public este configurat ca domeniu intern de retransmisie în loc de o domeniu de autoritate:

1. Deschideţi [Centrul de administrare Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Du-te la **fluxul de corespondenţă** \> **acceptat domenii**, selectaţi domeniul acceptat, şi apoi faceţi clic pe **Editare**.

3. În proprietăţile paginii care se deschide, în cazul în care tipul de domeniu este setată la **Authoritative**, value la spre **intern de retransmisie** şi apoi faceţi clic pe **salvaţi**.

Dacă expeditori externi primesc eroare, **nu aveţi permisiunea (550 5.7.13)**, executaţi comanda următoare în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi în folderul public:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Pentru a permite utilizatorilor externi să trimite email pentru acest folder public, Adauga acces CreateItems dreptul la utilizator anonim. De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
