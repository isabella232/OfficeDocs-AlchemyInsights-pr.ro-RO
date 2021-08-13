---
title: Mutarea mesajelor de e-mail în cutia poștală Arhivă
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974969"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mutați e-mailul în cutia poștală de arhivare

Dacă doriți să rulați verificări automate pentru setările menționate mai jos, selectați butonul Înapoi < - în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme la mutarea e-mailului în cutia poștală de arhivare.

1. Confirmați că a **fost activată** o cutie poștală de arhivare. Dacă nu, urmați pașii din acest [articol pentru a](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) activa cutia poștală de arhivare.

2. Pentru a arhiva automat mesajele în cutia  poștală de arhivare, o etichetă de retenție cu acțiunea Mutați în arhivă trebuie setată să se aplice automat la întreaga etichetă cutie poștală **(implicită).** Utilizați pașii de aici pentru a crea eticheta: [Eticheta implicită Arhivare](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. În continuare, adăugați eticheta **Arhivă la** politica de retenție. În centrul Exchange, alegeți  Politici de retenție > a adăuga eticheta Mutare la **arhivare** la politica > **Salvare.**

4. Acum [atribuiți Politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cutiei poștale a utilizatorului specific. Aceeași politică se va aplica atât cutiei **poștale principale,** cât și **cutiei poștale de** arhivare.

Poate fi necesar să impuneți Asistentului pentru foldere gestionate (MFA) să ruleze și să aplice setările noi la cutia poștală a utilizatorului. Rulați următoarea comandă în timp [ce sunteți conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni Asistentul de foldere gestionate pentru o anumită cutie poștală:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Pentru mai multe informații despre configurarea unei politici de arhivare, consultați Configurarea unei politici de arhivare și [de ștergere pentru cutiile poștale.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  