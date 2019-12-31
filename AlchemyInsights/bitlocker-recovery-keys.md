---
title: Taste de recuperare BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908826"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="396ce-102">Accesarea tastelor de recuperare BitLocker</span><span class="sxs-lookup"><span data-stu-id="396ce-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="396ce-103">Când configurați setările BitLocker Intune Endpoint protecția politica, este posibil să se definească dacă informațiile de recuperare BitLocker ar trebui să fie stocate în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="396ce-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="396ce-104">Dacă setarea este configurată, datele de recuperare stocate ar trebui să fie vizibile pentru un administrator Intune ca parte a datelor de înregistrare dispozitiv în lama dispozitive Intune în două moduri:</span><span class="sxs-lookup"><span data-stu-id="396ce-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="396ce-105">Dispozitive-dispozitive AD Azure-> "dispozitiv" sau dispozitive-> toate dispozitivele-> "Device"-> taste de recuperare</span><span class="sxs-lookup"><span data-stu-id="396ce-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="396ce-106">Alternativ, dacă există acces administrativ la dispozitivul în sine, cheia de recuperare (Password) poate fi văzută executând următoarea comandă dintr-un prompt de comandă privilegiat:</span><span class="sxs-lookup"><span data-stu-id="396ce-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="396ce-107">Dacă dispozitivul a fost criptat înainte de înscrierea în Intune, este posibil ca cheia de recuperare să fi fost asociată cu "contul Microsoft" (MSA) utilizat pentru a face sign in la dispozitiv în timpul procesului OOBE.</span><span class="sxs-lookup"><span data-stu-id="396ce-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="396ce-108">În cazul în care a fost cazul https://onedrive.live.com/recoverykey , accesarea și conectarea cu care MSA ar trebui să arate dispozitivele pentru care cheile de recuperare au fost stocate.</span><span class="sxs-lookup"><span data-stu-id="396ce-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="396ce-109">Dacă dispozitivul a fost criptat ca urmare a configurării prin Politica de grup bazată pe domeniu, informațiile de recuperare pot fi stocate în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="396ce-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

