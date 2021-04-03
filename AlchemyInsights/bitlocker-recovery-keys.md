---
title: Chei de recuperare BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505080"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="e5e7f-102">Accesarea cheilor de recuperare BitLocker</span><span class="sxs-lookup"><span data-stu-id="e5e7f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="e5e7f-103">Atunci când configurați setările Bitlocker Politica de protecție Intune Endpoint, este posibil să definiți dacă informațiile de recuperare Bitlocker trebuie să fie stocate în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e5e7f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="e5e7f-104">Dacă această setare este configurată, datele de recuperare stocate trebuie să fie vizibile pentru un administrator Intune ca parte a datelor înregistrării dispozitivului în blade pentru dispozitive Intune în două moduri:</span><span class="sxs-lookup"><span data-stu-id="e5e7f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="e5e7f-105">Dispozitive - dispozitive Azure AD -> "Dispozitiv" SAU Dispozitive -> Toate dispozitivele -> "Dispozitiv" -> Recuperare</span><span class="sxs-lookup"><span data-stu-id="e5e7f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="e5e7f-106">Ca alternativă, dacă există acces administrativ la dispozitivul propriu-zis, cheia de recuperare (Parolă) poate fi văzută rulezând următoarea comandă dintr-o linie de comandă cu drepturi elevate:</span><span class="sxs-lookup"><span data-stu-id="e5e7f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="e5e7f-107">Dacă dispozitivul a fost criptat înainte de înscrierea în Intune, este posibil ca cheia de recuperare să fi fost asociată cu "Cont Microsoft" (MSA) utilizată pentru a se conecta la dispozitiv în timpul procesului OOBE.</span><span class="sxs-lookup"><span data-stu-id="e5e7f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="e5e7f-108">Dacă acesta a fost cazul, accesarea și conectarea cu acel MSA ar trebui să arate dispozitivele pentru  https://onedrive.live.com/recoverykey care s-au stocat cheile de recuperare.</span><span class="sxs-lookup"><span data-stu-id="e5e7f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="e5e7f-109">În cazul în care dispozitivul a fost criptat ca rezultat al configurării prin politica de grup bazată pe domeniu, informațiile despre recuperare pot fi stocate în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="e5e7f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="e5e7f-110">Dacă ați configurat politica de protecție a punctului final pentru a stoca cheia de recuperare în Azure Active Directory, dar cheia pentru un anumit dispozitiv nu a fost încărcată, puteți declanșa încărcarea, rotind cheia de recuperare pentru acel dispozitiv din consola MEM.</span><span class="sxs-lookup"><span data-stu-id="e5e7f-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="e5e7f-111">Pentru detalii, consultați Rotire [chei de recuperare BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="e5e7f-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

