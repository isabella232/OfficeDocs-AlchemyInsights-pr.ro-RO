---
title: Chei de recuperare BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060076"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accesarea cheilor de recuperare BitLocker

Atunci când configurați setările BitLocker Politica Endpoint Protection Intune, este posibil să definiți dacă informațiile de recuperare Bitlocker trebuie să fie stocate în Azure Active Directory.

Dacă această setare este configurată, datele de recuperare stocate trebuie să fie vizibile pentru un administrator Intune ca parte a datelor înregistrării dispozitivului în blade pentru dispozitive Intune în două moduri:

Dispozitive - dispozitive Azure AD -> "Dispozitiv" SAU Dispozitive -> Toate dispozitivele -> "Dispozitiv" -> Recuperare

Ca alternativă, dacă există acces administrativ la dispozitivul propriu-zis, cheia de recuperare (Parolă) poate fi văzută rulezând următoarea comandă dintr-o linie de comandă cu drepturi elevate:

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
Dacă dispozitivul a fost criptat înainte de înscrierea în Intune, este posibil ca cheia de recuperare să fi fost asociată cu "Cont Microsoft" (MSA) utilizată pentru a se conecta la dispozitiv în timpul procesului OOBE. Dacă acesta a fost cazul, accesarea și conectarea cu acel MSA ar trebui să arate dispozitivele pentru  https://onedrive.live.com/recoverykey care s-au stocat cheile de recuperare.
 
În cazul în care dispozitivul a fost criptat ca rezultat al configurării prin politica de grup bazată pe domeniu, informațiile despre recuperare pot fi stocate în Active Directory local.

Dacă ați configurat o politică de protecție pentru punctul final pentru a stoca cheia de recuperare în Azure Active Directory dar cheia pentru un anumit dispozitiv nu a fost încărcată, puteți declanșa încărcarea, rotind cheia de recuperare pentru acel dispozitiv din consola MEM. Pentru detalii, consultați Rotire [chei de recuperare BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

