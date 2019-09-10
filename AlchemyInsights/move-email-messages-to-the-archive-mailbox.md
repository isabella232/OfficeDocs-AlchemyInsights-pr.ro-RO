---
title: Mutarea mesajelor de poștă electronică în cutia poștală arhivă
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822174"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mutarea e-mailului în cutia poștală arhivă

1. Confirmați că a fost activată o **cutie poștală arhivă** . Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pentru a activa cutia poștală de arhivă.

2. Pentru a arhiva mesajele automat la cutia poștală de arhivă, o etichetă de retenție cu **Mutare în arhivă** acțiune trebuie setată la **aplicată automat la întreaga cutie poștală (implicit) etichetă**. Utilizați pașii de aici pentru a crea eticheta: [arhivați eticheta implicită](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Apoi, adăugați eticheta de **arhivă** la Politica de retenție. În centrul de administrare Exchange, alegeți **politicile de conservare** > adăugați **mutați în arhiva etichetă** la politica > **Salvare**.

4. Acum [atribuiți Politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poștală a utilizatorului specific. Aceeași politică se va aplica atât la cutia poștală **principală** și **arhivă** .

Poate fi necesar să forțați asistentul pentru foldere gestionate (MFA) să ruleze și să aplice noile setări la cutia poștală a utilizatorului. Executați următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul de foldere gestionate pentru o anumită cutie poștală:
  
Start-ManagedFolderAssistant-identitate<name of the mailbox>

Pentru mai multe informații despre configurarea unei politici de arhivă, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  