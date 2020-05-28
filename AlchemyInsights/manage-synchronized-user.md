---
title: Gestionare utilizator sincronizat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407362"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Imposibil de setat adresa de e-mail principală, de a modifica atributele utilizatorului sau de a elimina/șterge un utilizator sincronizat

Dacă sincronizarea directorului este activată pentru mediul dvs., unele atribute de utilizator sau obiect nu se pot modifica utilizând centrul de administrare Microsoft 365.

Pentru a gestiona complet utilizatorii sincronizați și toate atributele lor, utilizați consola de gestionare locală a utilizatorilor active directory și a grupurilor (adsiedit.msc).  

Alternativ, aveți posibilitatea să modificați utilizatori individuali sau atribute pentru utilizatorii sincronizați utilizând PowerShell, se arată în aceste exemple obișnuite: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
