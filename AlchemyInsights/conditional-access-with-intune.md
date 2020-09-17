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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807671"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f8ccd-102">Acces condiționat cu Intune</span><span class="sxs-lookup"><span data-stu-id="f8ccd-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f8ccd-103">Utilizarea  **accesului condiționat**  cu Intune necesită 3 pași:</span><span class="sxs-lookup"><span data-stu-id="f8ccd-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f8ccd-104">Creați o  **politică de conformitate**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f8ccd-105">De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat conform.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f8ccd-106">Creați o **politică de acces condiționat**  care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa acele resurse.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f8ccd-107">[De exemplu,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul corporativ.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f8ccd-108">Asigurați-vă că **politicile de conformitate**  și  **politicile de acces condiționat**  sunt direcționate către grupurile dorite de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f8ccd-109">Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8ccd-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f8ccd-110">**Linkuri utile:**</span><span class="sxs-lookup"><span data-stu-id="f8ccd-110">**Helpful links:**</span></span>

[<span data-ttu-id="f8ccd-111">Prezentare generală a conformității dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="f8ccd-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f8ccd-112">Depanarea CA</span><span class="sxs-lookup"><span data-stu-id="f8ccd-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f8ccd-113">Politica de depanare</span><span class="sxs-lookup"><span data-stu-id="f8ccd-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f8ccd-114">Pentru a proteja e-mailul (Exchange Online) de la acces la dispozitive neconforme, trebuie respectate ambele documente:</span><span class="sxs-lookup"><span data-stu-id="f8ccd-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f8ccd-115">Protejarea accesului la e-mail de pe dispozitive utilizând EAS</span><span class="sxs-lookup"><span data-stu-id="f8ccd-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f8ccd-116">Protejarea accesului la e-mail de pe dispozitive utilizând clienți moderni de autentificare, cum ar fi Outlook</span><span class="sxs-lookup"><span data-stu-id="f8ccd-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)