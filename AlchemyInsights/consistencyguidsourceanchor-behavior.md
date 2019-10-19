---
title: Comportamentul ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36517006"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="1e698-102">Comportamentul ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="1e698-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="1e698-103">Azure AD Connect (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca sourceAnchor atribut.</span><span class="sxs-lookup"><span data-stu-id="1e698-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="1e698-104">Când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare la:</span><span class="sxs-lookup"><span data-stu-id="1e698-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="1e698-105">Utilizați msDS-ConsistencyGuid ca atributul sourceAnchor pentru obiectele de utilizator.</span><span class="sxs-lookup"><span data-stu-id="1e698-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="1e698-106">ObjectGUID este utilizat pentru alte tipuri de obiecte.</span><span class="sxs-lookup"><span data-stu-id="1e698-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="1e698-107">Pentru orice anumit obiect de utilizator AD local al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect scrie valoarea objectGUID înapoi la atributul msDS-ConsistencyGuid în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="1e698-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="1e698-108">După atributul msDS-ConsistencyGuid este populat, Azure AD Connect apoi exportă obiectul Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e698-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="1e698-109">**Notă:** Odată ce un obiect AD local este importat în Azure AD Connect (care este, importate în spațiul de conector AD și proiectate în metaverse), nu se poate modifica valoarea sourceAnchor mai.</span><span class="sxs-lookup"><span data-stu-id="1e698-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="1e698-110">Pentru a specifica valoarea sourceAnchor pentru un anumit obiect AD local, configurați atributul msDS-ConsistencyGuid înainte de a fi importate în Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1e698-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="1e698-111">Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [AZURE AD Connect: concepte de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="1e698-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

