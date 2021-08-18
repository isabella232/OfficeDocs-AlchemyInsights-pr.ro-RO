---
title: Gestionare utilizator sincronizat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114790"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Imposibil de setat adresa de e-mail principală, de a modifica atributele de utilizator sau de a elimina/șterge un utilizator sincronizat

Dacă sincronizarea directorului este activată pentru mediul dvs., unele atribute de utilizator sau de obiect nu pot fi modificate utilizând Centru de administrare Microsoft 365.

Pentru a gestiona complet utilizatorii sincronizați și toate atributele lor, utilizați utilizatorii Local Active Directory și consola de gestionare a grupurilor (adsiedit.msc).  

Alternativ, puteți modifica utilizatorii individuali sau atributele pentru utilizatorii sincronizați folosind powershell, cum ar fi cele afișate în aceste exemple comune:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
