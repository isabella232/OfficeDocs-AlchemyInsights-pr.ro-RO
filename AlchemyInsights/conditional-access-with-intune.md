---
title: Acces condiționat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505006"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8ad7c-102">Acces condiționat cu Intune</span><span class="sxs-lookup"><span data-stu-id="8ad7c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8ad7c-103">Utilizarea **condițională de acces** cu Intune necesită 3 pași:</span><span class="sxs-lookup"><span data-stu-id="8ad7c-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="8ad7c-104">Creați o **politică de acces condiționată** care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa aceste resurse.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="8ad7c-105">De exemplu, un dispozitiv trebuie să fie conforme înainte de accesarea e-mailului corporativ.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="8ad7c-106">Creați o **politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat conform.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="8ad7c-107">De exemplu, un dispozitiv trebuie să aibă un PIN de cel puțin 6 cifre înainte de a fi considerat compatibil.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="8ad7c-108">Asigurarea **respectării politicilor de conformitate** și a **politicilor de acces condițional** sunt direcționate către grupurile dorite de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="8ad7c-109">Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8ad7c-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="8ad7c-110">Citeste mai mult:</span><span class="sxs-lookup"><span data-stu-id="8ad7c-110">Read more:</span></span>
  
- [<span data-ttu-id="8ad7c-111">Cele mai bune practici de acces condiționat</span><span class="sxs-lookup"><span data-stu-id="8ad7c-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="8ad7c-112">Noțiuni introductive despre accesul condiționat</span><span class="sxs-lookup"><span data-stu-id="8ad7c-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

