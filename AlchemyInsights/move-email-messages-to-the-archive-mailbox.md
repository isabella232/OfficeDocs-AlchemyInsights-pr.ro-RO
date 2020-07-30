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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522783"
---
# <a name="move-email-to-the-archive-mailbox"></a>Mutarea e-mailului în cutia poștală de arhivă

Dacă doriți să executăm verificări automate pentru setările menționate mai jos, selectați butonul din spate <-- în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme în mutarea e-mailului în cutia poștală de arhivă.

1. Confirmați că a fost activată o **cutie poștală Arhivă.** Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) pentru a activa cutia poștală de arhivă.

2. Pentru a arhiva automat mesajele în cutia poștală de arhivă, o etichetă de retenție cu acțiunea **Mutare în arhivă** trebuie setată automat la eticheta **aplicată automat întregii cutii poștale (implicit).** Utilizați pașii de aici pentru a crea eticheta: [Arhivați eticheta implicită](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Apoi, adăugați eticheta **Arhivă** la politica de retenție. În centrul de administrare Exchange, alegeți **Politici de retenție** > **adăugați eticheta Mutare la arhivă** la politica > **Salvare**.

4. Acum [atribuiți politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cutiei poștale a utilizatorului respectiv. Aceeași politică se va aplica atât cutiei **poștale Primară,** cât și cutiei poștale **Arhivă.**

Poate fi necesar să forțați Asistentul de foldere gestionate (MFA) să ruleze și să aplice noile setări cutiei poștale a utilizatorului. Executați următoarea comandă în timp ce [sunteți conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni Asistentul de foldere gestionate pentru o anumită cutie poștală:
  
Pornire-gestionatFolderAssistant -Identitate<name of the mailbox>

Pentru mai multe informații despre configurarea unei politici de arhivă, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  