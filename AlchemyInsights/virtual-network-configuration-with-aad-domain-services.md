---
title: Configurație virtuală cu servicii de domeniu AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885647"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="d177b-102">Configurație virtuală cu servicii de domeniu AAD</span><span class="sxs-lookup"><span data-stu-id="d177b-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="d177b-103">Configurarea virtuală cu servicii de domeniu AAD implică următorii pași:</span><span class="sxs-lookup"><span data-stu-id="d177b-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="d177b-104">Verificarea stării domeniului în portalul Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="d177b-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="d177b-105">Verificarea NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în Azure AD Domain Services pe portal https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="d177b-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="d177b-106">Pentru a vă asigura că rețeaua virtuală este implementată în aceeași regiune Azure ca domeniu gestionat de domeniul Azure AD Services.</span><span class="sxs-lookup"><span data-stu-id="d177b-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="d177b-107">Pentru a vă asigura că nu aveți un domeniu existent cu același nume de domeniu disponibil în rețeaua virtuală.</span><span class="sxs-lookup"><span data-stu-id="d177b-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="d177b-108">Pentru mai multe detalii despre proiectarea aspectului în rețeaua virtuală Azure pentru a accepta servicii de domeniu AAD, consultați [analiza rețelelor virtuale](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="d177b-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

