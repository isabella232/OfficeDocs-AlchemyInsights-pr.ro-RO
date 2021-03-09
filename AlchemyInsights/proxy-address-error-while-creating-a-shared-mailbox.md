---
title: Eroare de adresă proxy în timp ce creați o cutie poștală partajată
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568302"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Eroare de adresă proxy în timp ce creați o cutie poștală sau alt obiect activat pentru e-mail

Dacă ați încercat să creați un obiect activat pentru e-mail (cutie poștală, cutie poștală partajată etc.) și ați primit eroarea "adresa proxy" SMTP:alias@domain.com "este deja utilizată...", adresa de e-mail pe care ați ales-o este deja luată de un alt obiect activat pentru e-mail din organizația dvs.
  
Trebuie să găsiți utilizatorul, grupul, cutia poștală partajată sau folderul public care are această adresă de e-mail și să o șteargă sau să își modifice adresa de e-mail. Apoi puteți crea un nou obiect activat pentru e-mail cu adresa de e-mail gratuită. Utilizați căutare pe pagina de pornire pentru a o găsi. De asemenea, puteți utiliza următoarea comandă PowerShell Exchange Online pentru a o căuta:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Dacă nu doriți să ștergeți adresa de e-mail existentă, alegeți o nouă adresă de e-mail pentru obiectul nou pe care îl creați.
  