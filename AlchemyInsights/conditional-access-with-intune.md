---
title: Acces condiționat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931448"
---
# <a name="conditional-access-with-intune"></a>Acces condiționat cu Intune

Utilizarea **accesului condiționat** cu Intune necesită 3 pași:

- Creați o **politică de conformitate** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat compatibil. De exemplu, un dispozitiv trebuie să aibă un ac de cel puțin 6 cifre înainte de a fi considerat conform.
- Creați o **politică de acces condiționat** care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa aceste resurse.  [De exemplu,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul companiei.
- Asigurați-vă că atât **politicile de conformitate,** cât și **politicile de acces condiționat** sunt direcționate către grupurile de utilizatori dorite. Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.

**Link-uri utile:**

[Prezentare generală a conformității dispozitivelor](https://docs.microsoft.com/intune/device-compliance-get-started)

[Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politica de depanare](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Pentru a proteja e-mailul (Exchange online) de accesul dispozitivelor neconforme, ambele documente trebuie urmate:

1. [Protejarea accesului la e-mail împotriva dispozitivelor care utilizează EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protejarea accesului la e-mail de dispozitive utilizând clienți de autentificare moderni, ar fi Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)