---
title: ConsistențăGuid /sourceAnchor behavior
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817004"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d8357-102">ConsistențăGuid /sourceAnchor behavior</span><span class="sxs-lookup"><span data-stu-id="d8357-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d8357-103">Azure AD Connect (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d8357-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d8357-104">Atunci când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare la:</span><span class="sxs-lookup"><span data-stu-id="d8357-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d8357-105">Utilizați msDS-ConsistencyGuid ca atribut sourceAnchor pentru obiectele User.</span><span class="sxs-lookup"><span data-stu-id="d8357-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d8357-106">ObjectGUID este utilizat pentru alte tipuri de obiecte.</span><span class="sxs-lookup"><span data-stu-id="d8357-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d8357-107">Pentru orice obiect AD User local dat al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect își scrie valoarea objectGUID înapoi în atributul msDS-ConsistencyGuid în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="d8357-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d8357-108">După ce este populat atributul msDS-ConsistencyGuid, Azure AD Connect exportă apoi obiectul în Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8357-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d8357-109">**Notă:** După ce un obiect AD local este importat în Azure AD Connect (care este importat în Spațiul conectorului AD și proiectat în Metaversu), nu îi mai puteți modifica valoarea sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="d8357-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d8357-110">Pentru a specifica valoarea sourceAnchor pentru un anumit obiect AD local, configurați atributul msDS-ConsistencyGuid înainte ca acesta să fie importat în Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d8357-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d8357-111">Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [Azure AD Connect: Concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d8357-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

