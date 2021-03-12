---
title: Acces condiționat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704798"
---
# <a name="conditional-access-with-intune"></a>Acces condiționat cu Intune

Utilizarea  **accesului condiționat**  cu Intune necesită 3 pași:

- Creați o  **politică de conformitate**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat conform.
- Creați o **politică de acces condiționat**  care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa acele resurse.  [De exemplu,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul corporativ.
- Asigurați-vă că **politicile de conformitate**  și  **politicile de acces condiționat**  sunt direcționate către grupurile dorite de utilizatori. Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.

**Linkuri utile:**

[Prezentare generală a conformității dispozitivelor](https://docs.microsoft.com/intune/device-compliance-get-started)

[Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politica de depanare](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Pentru a proteja e-mailul (Exchange Online) de la acces la dispozitive neconforme, trebuie respectate ambele documente:

1. [Protejarea accesului la e-mail de pe dispozitive utilizând EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protejarea accesului la e-mail de pe dispozitive utilizând clienți moderni de autentificare, cum ar fi Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)