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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749260"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="e2eb0-102">Utilizarea accesului condiționat cu Intune</span><span class="sxs-lookup"><span data-stu-id="e2eb0-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="e2eb0-103">Utilizarea accesului condiționat cu Intune necesită 3 pași:</span><span class="sxs-lookup"><span data-stu-id="e2eb0-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="e2eb0-104">Creați o politică de conformitate pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform. De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat conform.</span><span class="sxs-lookup"><span data-stu-id="e2eb0-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="e2eb0-105">Creați o politică de acces condiționat care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa acele resurse. De exemplu, un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul corporativ.</span><span class="sxs-lookup"><span data-stu-id="e2eb0-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="e2eb0-106">Asigurați-vă că politicile de conformitate și politicile de acces condiționat sunt direcționate către grupurile dorite de utilizatori. Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e2eb0-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e2eb0-107">Citiți mai multe...</span><span class="sxs-lookup"><span data-stu-id="e2eb0-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
