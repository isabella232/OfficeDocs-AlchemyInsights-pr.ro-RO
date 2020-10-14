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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="3aeee-102">Nu puteți să setați adresa de e-mail principală, să modificați atributele utilizatorilor sau să eliminați/să ștergeți un utilizator sincronizat</span><span class="sxs-lookup"><span data-stu-id="3aeee-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="3aeee-103">Dacă sincronizarea directoarelor este activată pentru mediul dvs., unele atribute de utilizator sau obiect nu pot fi modificate utilizând Centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3aeee-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="3aeee-104">Pentru a gestiona pe deplin utilizatorii sincronizați și toate atributele lor, utilizați consola de gestionare a utilizatorilor și grupurilor Active Directory locale (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="3aeee-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="3aeee-105">Ca alternativă, puteți să modificați utilizatori individuali sau atribute pentru utilizatorii sincronizați utilizând PowerShell, cum ar fi afișate în aceste exemple comune:</span><span class="sxs-lookup"><span data-stu-id="3aeee-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
