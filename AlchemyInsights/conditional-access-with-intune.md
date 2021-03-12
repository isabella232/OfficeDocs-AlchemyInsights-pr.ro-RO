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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="237a3-102">Acces condiționat cu Intune</span><span class="sxs-lookup"><span data-stu-id="237a3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="237a3-103">Utilizarea  **accesului condiționat**  cu Intune necesită 3 pași:</span><span class="sxs-lookup"><span data-stu-id="237a3-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="237a3-104">Creați o  **politică de conformitate**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform.</span><span class="sxs-lookup"><span data-stu-id="237a3-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="237a3-105">De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat conform.</span><span class="sxs-lookup"><span data-stu-id="237a3-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="237a3-106">Creați o **politică de acces condiționat**  care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa acele resurse.</span><span class="sxs-lookup"><span data-stu-id="237a3-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="237a3-107">[De exemplu,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul corporativ.</span><span class="sxs-lookup"><span data-stu-id="237a3-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="237a3-108">Asigurați-vă că **politicile de conformitate**  și  **politicile de acces condiționat**  sunt direcționate către grupurile dorite de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="237a3-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="237a3-109">Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="237a3-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="237a3-110">**Linkuri utile:**</span><span class="sxs-lookup"><span data-stu-id="237a3-110">**Helpful links:**</span></span>

[<span data-ttu-id="237a3-111">Prezentare generală a conformității dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="237a3-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="237a3-112">Depanarea CA</span><span class="sxs-lookup"><span data-stu-id="237a3-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="237a3-113">Politica de depanare</span><span class="sxs-lookup"><span data-stu-id="237a3-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="237a3-114">Pentru a proteja e-mailul (Exchange Online) de la acces la dispozitive neconforme, trebuie respectate ambele documente:</span><span class="sxs-lookup"><span data-stu-id="237a3-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="237a3-115">Protejarea accesului la e-mail de pe dispozitive utilizând EAS</span><span class="sxs-lookup"><span data-stu-id="237a3-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="237a3-116">Protejarea accesului la e-mail de pe dispozitive utilizând clienți moderni de autentificare, cum ar fi Outlook</span><span class="sxs-lookup"><span data-stu-id="237a3-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)