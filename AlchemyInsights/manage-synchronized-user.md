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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380517"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="fe756-102">Imposibil de setat adresa de email primar sau schimba atributele utilizatorilor</span><span class="sxs-lookup"><span data-stu-id="fe756-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="fe756-103">În cazul în care sincronizarea directorului este activată pentru mediul de unele atribute de utilizator sau un obiect nu poate fi schimbat, utilizând Centrul de administrare.</span><span class="sxs-lookup"><span data-stu-id="fe756-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="fe756-104">Pentru a gestiona complet sincronizate utilizatorii şi toate atributele lor, utilizaţi dumneavoastră locale active Director utilizatori și grupuri consola de gestionare (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="fe756-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="fe756-105">Alternativ, puteţi să schimbaţi utilizatorii individuali sau atribute pentru utilizatorii sincronizate folosind powershell cum ar fi arătat în aceste exemple comune:</span><span class="sxs-lookup"><span data-stu-id="fe756-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="fe756-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fe756-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="fe756-107">Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test utilizator" - Prenume "Utilizator"-titlul de "Manager"-Departamentul "HR"</span><span class="sxs-lookup"><span data-stu-id="fe756-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="fe756-108">Remove-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="fe756-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>