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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="5a4d4-102">Imposibil de setat adresa de e-mail principală, de a modifica atributele utilizatorului sau de a elimina/șterge un utilizator sincronizat</span><span class="sxs-lookup"><span data-stu-id="5a4d4-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="5a4d4-103">Dacă sincronizarea directorului este activată pentru mediul dvs., unele atribute de utilizator sau obiect nu se pot modifica utilizând centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5a4d4-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="5a4d4-104">Pentru a gestiona complet utilizatorii sincronizați și toate atributele lor, utilizați consola de gestionare locală a utilizatorilor active directory și a grupurilor (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="5a4d4-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="5a4d4-105">Alternativ, aveți posibilitatea să modificați utilizatori individuali sau atribute pentru utilizatorii sincronizați utilizând PowerShell, se arată în aceste exemple obișnuite:</span><span class="sxs-lookup"><span data-stu-id="5a4d4-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
