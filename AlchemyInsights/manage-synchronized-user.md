---
title: Gestiona sincronizate utilizator
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542013"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="24424-102">Imposibil de setat adresa de email primar sau schimba atributele utilizatorilor</span><span class="sxs-lookup"><span data-stu-id="24424-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="24424-103">În cazul în care sincronizarea directorului este activată pentru mediul, unele atribute de utilizator sau un obiect nu poate fi schimbat, utilizând Centrul de administrare Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="24424-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="24424-104">Pentru a gestiona complet sincronizate utilizatorii şi toate atributele lor, utilizaţi dumneavoastră locale active Director utilizatori și grupuri consola de gestionare (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="24424-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="24424-105">Alternativ, puteţi să schimbaţi utilizatorii individuali sau atribute pentru utilizatorii sincronizate folosind powershell cum ar fi arătat în aceste exemple comune:</span><span class="sxs-lookup"><span data-stu-id="24424-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="24424-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="24424-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="24424-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test utilizator" - Prenume "Utilizator"-titlul de "Manager"-Departamentul "HR"</span><span class="sxs-lookup"><span data-stu-id="24424-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="24424-108">Remove-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="24424-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>