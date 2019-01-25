---
title: Acces condiţionat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485618"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8ff96-102">Acces condiţionat cu Intune</span><span class="sxs-lookup"><span data-stu-id="8ff96-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8ff96-103">Folosind **Accesul condiționat** cu Intune necesită 3 pasi:</span><span class="sxs-lookup"><span data-stu-id="8ff96-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="8ff96-p101">Creaţi o **Politica de acces condiționat** , care defineşte ce resurse sunt protejata, şi ce condiţii trebuie să fie îndeplinite pentru a accesa aceste resurse. De exemplu, un aparat trebuie să fie compatibile cu înainte de a accesa e-mail corporative.</span><span class="sxs-lookup"><span data-stu-id="8ff96-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="8ff96-p102">Creaţi o **Politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul este considerat compatibil cu. De exemplu, un aparat trebuie să aibă un ac de cel puţin 6 cifre înainte se consideră conforme.</span><span class="sxs-lookup"><span data-stu-id="8ff96-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="8ff96-p103">Asigura **Respectarea politicilor** şi de **Politici de acces condiționat** sunt direcţionate către grupuri dorit de utilizatori. Acest lucru poate necesita crearea grupuri specifice de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8ff96-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="8ff96-110">Citiți mai multe</span><span class="sxs-lookup"><span data-stu-id="8ff96-110">Read more:</span></span>
  
- [<span data-ttu-id="8ff96-111">Condiţionată de acces cele mai bune practici</span><span class="sxs-lookup"><span data-stu-id="8ff96-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="8ff96-112">Noţiuni de bază cu acces condiționat</span><span class="sxs-lookup"><span data-stu-id="8ff96-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

