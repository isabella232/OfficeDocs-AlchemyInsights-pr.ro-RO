---
title: Gestionarea unui utilizator sincronizat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777689"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nu puteți să setați adresa de e-mail principală, să modificați atributele utilizatorilor sau să eliminați/să ștergeți un utilizator sincronizat

Dacă sincronizarea directoarelor este activată pentru mediul dvs., unele atribute de utilizator sau obiect nu pot fi modificate utilizând Centrul de administrare Microsoft 365.

Pentru a gestiona pe deplin utilizatorii sincronizați și toate atributele lor, utilizați consola de gestionare a utilizatorilor și grupurilor Active Directory locale (ADSIEdit. msc).  

Ca alternativă, puteți să modificați utilizatori individuali sau atribute pentru utilizatorii sincronizați utilizând PowerShell, cum ar fi afișate în aceste exemple comune: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
