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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505006"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="27b6d-102">Acces condiţionat cu Intune</span><span class="sxs-lookup"><span data-stu-id="27b6d-102">Conditional Access with Intune</span></span>

<span data-ttu-id="27b6d-103">Folosind **Accesul condiționat** cu Intune necesită 3 pasi:</span><span class="sxs-lookup"><span data-stu-id="27b6d-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="27b6d-104">Creaţi o **Politica de acces condiționat** , care defineşte ce resurse sunt protejata, şi ce condiţii trebuie să fie îndeplinite pentru a accesa aceste resurse.</span><span class="sxs-lookup"><span data-stu-id="27b6d-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="27b6d-105">De exemplu, un aparat trebuie să fie compatibile cu înainte de a accesa e-mail corporative.</span><span class="sxs-lookup"><span data-stu-id="27b6d-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="27b6d-106">Creaţi o **Politică de conformitate** pentru a defini setările care trebuie îndeplinite înainte ca dispozitivul este considerat compatibil cu.</span><span class="sxs-lookup"><span data-stu-id="27b6d-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="27b6d-107">De exemplu, un aparat trebuie să aibă un ac de cel puţin 6 cifre înainte se consideră conforme.</span><span class="sxs-lookup"><span data-stu-id="27b6d-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="27b6d-108">Asigura **Respectarea politicilor** şi de **Politici de acces condiționat** sunt direcţionate către grupuri dorit de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="27b6d-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="27b6d-109">Acest lucru poate necesita crearea grupuri specifice de utilizatori în Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="27b6d-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="27b6d-110">Citeşte mai mult:</span><span class="sxs-lookup"><span data-stu-id="27b6d-110">Read more:</span></span>
  
- [<span data-ttu-id="27b6d-111">Condiţionată de acces cele mai bune practici</span><span class="sxs-lookup"><span data-stu-id="27b6d-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="27b6d-112">Noţiuni de bază cu acces condiționat</span><span class="sxs-lookup"><span data-stu-id="27b6d-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

