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
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694711"
---
# <a name="using-conditional-access-with-intune"></a>Utilizarea accesului condiționat cu Intune

Utilizarea accesului condiționat cu Intune necesită 3 pași:

- [Creați o politică de conformitate pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat conform.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Creați o politică de acces condiționat care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa acele resurse. De exemplu, un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul corporativ.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Asigurați-vă că politicile de conformitate și politicile de acces condiționat sunt direcționate către grupurile dorite de utilizatori. Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Citiți mai multe...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
