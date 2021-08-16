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
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069724"
---
# <a name="conditional-access-with-intune"></a>Acces condiționat cu Intune

Utilizarea  **accesului condiționat**  cu Intune necesită 3 pași:

- Creați o **politică de conformitate** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat compatibil. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre pentru a fi considerat compatibil.
- Creați o **politică de acces condiționat**  care să definească resursele ce trebuie protejate și condițiile care să fie îndeplinite pentru a accesa resursele respective.  [De exemplu, un dispozitiv](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  trebuie să fie conform înainte de a accesa un e-mail de corporație.
- **Asigurați-vă că atât politicile de conformitate,** **cât și politicile de** acces condiționat sunt orientate către grupurile de utilizatori dorite. Acest lucru poate necesita crearea anumitor grupuri de utilizatori Azure Active Directory.

**Linkuri utile:**

[Prezentarea generală a conformității dispozitivului](https://docs.microsoft.com/intune/device-compliance-get-started)

[Depanarea CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politică de depanare](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Pentru a proteja e-mailul (Exchange online) de la acces pe dispozitive care nu sunt dependente, trebuie urmărite ambele documente:

1. [Protejarea accesului la e-mail de pe dispozitive utilizând EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protejați accesul la e-mail de pe dispozitivele care utilizează clienți de autentificare moderni, cum ar fi Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)