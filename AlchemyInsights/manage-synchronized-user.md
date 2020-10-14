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
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451412"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nu puteți să setați adresa de e-mail principală, să modificați atributele utilizatorilor sau să eliminați/să ștergeți un utilizator sincronizat

Dacă sincronizarea directoarelor este activată pentru mediul dvs., unele atribute de utilizator sau obiect nu pot fi modificate utilizând Centrul de administrare Microsoft 365.

Pentru a gestiona pe deplin utilizatorii sincronizați și toate atributele lor, utilizați consola de gestionare a utilizatorilor și grupurilor Active Directory locale (ADSIEdit. msc).  

Ca alternativă, puteți să modificați utilizatori individuali sau atribute pentru utilizatorii sincronizați utilizând PowerShell, cum ar fi afișate în aceste exemple comune:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
