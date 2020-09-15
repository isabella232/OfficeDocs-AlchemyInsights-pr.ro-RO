---
title: Cheile de recuperare BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685898"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accesarea cheilor de recuperare BitLocker

Atunci când configurați setările BitLocker pentru Politica de protejare Endpoint, este posibil să definiți dacă informațiile de recuperare BitLocker ar trebui să fie stocate în Azure Active Directory.

Dacă acea setare este configurată, datele de recuperare stocate ar trebui să fie vizibile pentru un administrator Intune, ca parte a datelor de înregistrare a dispozitivului în Blade Devices Intune în două moduri:

Dispozitive-dispozitive Azure AD-> "dispozitiv" sau dispozitive-> toate dispozitivele-> "dispozitiv"-cheile de recuperare >

Ca alternativă, dacă există acces administrativ la dispozitivul propriu-zis, cheia de recuperare (parolă) poate fi văzută rulând următoarea comandă dintr-un prompt de comandă privilegiat:

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
Dacă dispozitivul a fost criptat înainte de înscriere în Intune, cheia de recuperare poate fi asociată cu "contul Microsoft" (MSA) utilizat pentru a vă conecta la dispozitiv în timpul procesului OOBE. Dacă acesta a fost cazul, accesarea  https://onedrive.live.com/recoverykey și conectarea cu acel Sam trebuie să afișeze dispozitivele pentru care au fost stocate cheile de recuperare.
 
Dacă dispozitivul a fost criptat ca rezultat al configurării prin Politica de grup bazată pe domeniu, informațiile de recuperare pot fi stocate în Active Directory local.
 

