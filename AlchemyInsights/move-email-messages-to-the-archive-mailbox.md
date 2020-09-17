---
title: Mutarea mesajelor de e-mail în cutia poștală de arhivă
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799792"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mutarea e-mailului în cutia poștală arhivă

Dacă doriți să efectuăm verificări automate pentru setările menționate mai jos, selectați butonul înapoi <-în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu mutarea e-mailului în cutia poștală de arhivă.

1. Confirmați că a fost activată o **cutie poștală de arhivă** . Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) pentru a activa cutia poștală de arhivă.

2. Pentru a arhiva mesajele automat în cutia poștală de arhivă, o etichetă de retenție cu acțiunea **Mutare în arhivare** trebuie să fie setată la **aplicată automat la întreaga cutie poștală (implicită)**. Utilizați pașii de aici pentru a crea eticheta: [eticheta implicită arhivare](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Apoi, adăugați eticheta **arhivă** la Politica de retenție. În centrul de administrare Exchange, alegeți **politici de retenție** > adăugarea **etichetei mutare la arhivă** la politica > **Salvare**.

4. Acum [atribuiți Politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) în cutia poștală a utilizatorului respectiv. Aceeași politică se va aplica atât pentru cutia poștală **principală** , cât și pentru **arhivă** .

Poate fi necesar să Impuneți asistentul pentru foldere gestionate (AMF) pentru a executa și a aplica noile setări la cutia poștală a utilizatorului. Rulează următoarea comandă în timp ce [sunteți conectat la exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul de foldere gestionate pentru o anumită cutie poștală:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Pentru mai multe informații despre configurarea unei politici de arhivare, consultați [Configurarea unei politici de arhivare și de ștergere pentru cutiile poștale](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  