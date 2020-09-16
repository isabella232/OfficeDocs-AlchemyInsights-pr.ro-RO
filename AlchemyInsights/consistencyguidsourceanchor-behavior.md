---
title: Comportamentul ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756295"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3eff4-102">Comportamentul ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="3eff4-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3eff4-103">Azure AD Connect (versiunea 1.1.524.0 și After) facilitează acum utilizarea AMS-ConsistencyGuid ca atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3eff4-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3eff4-104">Atunci când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare pentru:</span><span class="sxs-lookup"><span data-stu-id="3eff4-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3eff4-105">Utilizați AMS-ConsistencyGuid ca atribut sourceAnchor pentru obiectele de utilizator.</span><span class="sxs-lookup"><span data-stu-id="3eff4-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3eff4-106">ObjectGUID este utilizat pentru alte tipuri de obiecte.</span><span class="sxs-lookup"><span data-stu-id="3eff4-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3eff4-107">Pentru orice obiect de utilizator de publicitate local al cărui atribut AMS-ConsistencyGuid nu este populat, Azure AD Connect își scrie valoarea objectGUID înapoi la atributul AMS-ConsistencyGuid în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="3eff4-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3eff4-108">După ce atributul AMS-ConsistencyGuid este populat, Azure AD Connect exportă obiectul la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3eff4-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3eff4-109">**Notă:** După ce un obiect de publicitate local este importat în Azure AD Connect (adică importat în spațiul conectorului de publicitate și proiectat în metaverse), nu mai puteți modifica valoarea sa sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3eff4-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3eff4-110">Pentru a specifica valoarea sourceAnchor pentru un anumit obiect de publicitate local, configurați atributul său AMS-ConsistencyGuid înainte de a fi importat în Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3eff4-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3eff4-111">Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [AZURE AD Connect: concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3eff4-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

