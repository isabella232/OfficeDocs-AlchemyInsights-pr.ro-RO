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
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706033"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="59c80-102">Acces condiționat cu Intune</span><span class="sxs-lookup"><span data-stu-id="59c80-102">Conditional Access with Intune</span></span>

<span data-ttu-id="59c80-103">Utilizarea **accesului condiționat** cu Intune necesită 3 pași:</span><span class="sxs-lookup"><span data-stu-id="59c80-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="59c80-104">Creați o **politică de acces condiționat** care definește ce resurse sunt protejate și ce condiții trebuie îndeplinite pentru a accesa aceste resurse.</span><span class="sxs-lookup"><span data-stu-id="59c80-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="59c80-105">De exemplu, un dispozitiv trebuie să fie compatibil înainte de a accesa e-mailul companiei.</span><span class="sxs-lookup"><span data-stu-id="59c80-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="59c80-106">Creați o **politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul să fie considerat compatibil.</span><span class="sxs-lookup"><span data-stu-id="59c80-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="59c80-107">De exemplu, un dispozitiv trebuie să aibă un cod PIN de cel puțin 6 cifre înainte de a fi considerat compatibil.</span><span class="sxs-lookup"><span data-stu-id="59c80-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="59c80-108">Asigurarea atât **a politicilor de conformitate,** cât și **a politicilor de acces condiționat** sunt direcționate către grupurile de utilizatori dorite.</span><span class="sxs-lookup"><span data-stu-id="59c80-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="59c80-109">Acest lucru poate necesita crearea anumitor grupuri de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59c80-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="59c80-110">Citește și...</span><span class="sxs-lookup"><span data-stu-id="59c80-110">Read more:</span></span>
  
- [<span data-ttu-id="59c80-111">Cele mai bune practici de acces condiționat</span><span class="sxs-lookup"><span data-stu-id="59c80-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="59c80-112">Introducere în Accesul condiționat</span><span class="sxs-lookup"><span data-stu-id="59c80-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

