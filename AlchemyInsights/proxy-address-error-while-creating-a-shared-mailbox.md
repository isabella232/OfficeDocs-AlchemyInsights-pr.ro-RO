---
title: Eroare de adresă proxy în timpul creării unei cutii poștale partajate
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062920"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Eroare de adresă proxy în timpul creării unei cutii poștale sau a unui alt obiect cu e-mail activat

Dacă ați încercat să creați un obiect cu e-mail activat (cutie poștală, cutie poștală partajată etc.) și ați primit eroarea "Adresa proxy "SMTP:alias@domain.com" este utilizată deja...", adresa de e-mail pe care ați ales-o este luată deja de alt obiect cu e-mail activat din organizația dvs.
  
Trebuie să găsiți utilizatorul, grupul, cutia poștală partajată sau folderul public care are această adresă de e-mail și să o ștergeți sau să-i modificați adresa de e-mail. Apoi puteți crea un obiect nou cu e-mail activat cu adresa de e-mail eliberată. Utilizați Căutare în pagina de pornire pentru a o găsi. De asemenea, puteți utiliza următoarea Exchange Online PowerShell pentru a o căuta:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Dacă nu doriți să ștergeți adresa de e-mail existentă, alegeți o nouă adresă de e-mail pentru noul obiect pe care îl creați.
  