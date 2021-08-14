---
title: Utilizarea accesului condiționat cu Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005786"
---
# <a name="using-conditional-access-with-intune"></a>Utilizarea accesului condiționat cu Intune

Utilizarea accesului condiționat cu Intune necesită 3 pași:

- [Creați o politică de conformitate pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat compatibil. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre pentru a fi considerat compatibil.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Creați o politică de acces condiționat care să definească resursele ce trebuie protejate și condițiile care să fie îndeplinite pentru a accesa resursele respective. De exemplu, un dispozitiv trebuie să fie conform înainte de a accesa un e-mail de corporație.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Asigurați-vă că atât politicile de conformitate, cât și politicile de acces condiționat sunt orientate către grupurile de utilizatori dorite. Acest lucru poate necesita crearea anumitor grupuri de utilizatori Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Citiți mai multe...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
