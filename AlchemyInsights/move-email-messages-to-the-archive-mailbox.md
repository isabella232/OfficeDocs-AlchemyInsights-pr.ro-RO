---
title: Mutarea mesajelor de e-mail în cutia poștală Arhivă
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713658"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mutarea e-mailului în cutia poștală de arhivă

1. Confirmați că a fost activată o **cutie poștală arhivă.** Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pentru a activa cutia poștală arhivă.

2. Pentru a arhiva automat mesajele în cutia poștală de arhivă, trebuie setată o etichetă de retenție cu acțiunea **Mutare în arhivă,** care trebuie setată automat **la întreaga etichetă poștală (implicită).** Utilizați pașii de aici pentru a crea eticheta: [Eticheta implicită arhivă](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Apoi, adăugați eticheta **Arhivă** la politica de conservare. În centrul de administrare Exchange, alegeți **Politici de conservare** > **adăugați eticheta Mutare la arhivă** la politica > **Salvare**.

4. Acum [atribuiți politica de conservare](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poștală a utilizatorului specific. Aceeași politică se va aplica atât în **cutia poștală principală,** cât și în cutia poștală **arhivă.**

Poate fi necesar să forțați Asistentul de foldere gestionate (AMF) să execute și să aplice noile setări cutiei poștale a utilizatorului. Executați următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni Asistent folder gestionat pentru o anumită cutie poștală:
  
Identitate a unui folder gestionat de pornire<name of the mailbox>

Pentru mai multe informații despre configurarea unei politici de arhivare, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  