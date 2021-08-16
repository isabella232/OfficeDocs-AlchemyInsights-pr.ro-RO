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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068824"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Remedierea problemelor de livrare a mesajelor de e-mail în folderele publice activate pentru e-mail

Dacă expeditorii externi nu pot trimite mesaje în folderele dvs. publice activate pentru e-mail și expeditorii primesc eroarea: nu a fost găsit **(550 5.4.1),** verificați dacă domeniul de e-mail pentru folderul public este configurat ca domeniu releu intern în loc de domeniu de autoritate:

1. Deschideți Centrul [de Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Accesați Flux **de corespondență** \> **Domenii acceptate**, selectați domeniul acceptat, apoi faceți clic pe **Editare**.

3. În pagina de proprietăți care se deschide, dacă tipul de domeniu este setat la De **autoritate,** modificați valoarea la Retransmisie **internă,** apoi faceți clic pe **Salvare.**

Dacă expeditorii externi primesc eroarea pe care nu o **aveți (550 5.7.13),** rulați următoarea comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi din folderul public:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Pentru a permite utilizatorilor externi să trimită mesaje de e-mail către acest folder public, adăugați accesul CreateItems direct la utilizatorul anonim. De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
