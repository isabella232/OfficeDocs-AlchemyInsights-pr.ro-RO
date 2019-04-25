---
title: Acces condiţionat cu Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393553"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="78fa2-102">Acces condiţionat cu Intune</span><span class="sxs-lookup"><span data-stu-id="78fa2-102">Conditional Access with Intune</span></span>

<span data-ttu-id="78fa2-103">Folosind **Accesul condiționat** cu Intune necesită 3 pasi:</span><span class="sxs-lookup"><span data-stu-id="78fa2-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="78fa2-104">Creaţi o **Politica de acces condiționat** , care defineşte ce resurse sunt protejata, şi ce condiţii trebuie să fie îndeplinite pentru a accesa aceste resurse.</span><span class="sxs-lookup"><span data-stu-id="78fa2-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="78fa2-105">De exemplu, un aparat trebuie să fie compatibile cu înainte de a accesa e-mail corporative.</span><span class="sxs-lookup"><span data-stu-id="78fa2-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="78fa2-106">Creaţi o **Politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul este considerat compatibil cu.</span><span class="sxs-lookup"><span data-stu-id="78fa2-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="78fa2-107">De exemplu, un aparat trebuie să aibă un ac de cel puţin 6 cifre înainte se consideră conforme.</span><span class="sxs-lookup"><span data-stu-id="78fa2-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="78fa2-108">Asigura **Respectarea politicilor** şi de **Politici de acces condiționat** sunt direcţionate către grupuri dorit de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="78fa2-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="78fa2-109">Acest lucru poate necesita crearea grupuri specifice de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="78fa2-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="78fa2-110">Citeşte mai mult:</span><span class="sxs-lookup"><span data-stu-id="78fa2-110">Read more:</span></span>
  
- [<span data-ttu-id="78fa2-111">Condiţionată de acces cele mai bune practici</span><span class="sxs-lookup"><span data-stu-id="78fa2-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="78fa2-112">Noţiuni de bază cu acces condiționat</span><span class="sxs-lookup"><span data-stu-id="78fa2-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

