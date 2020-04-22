---
title: ConsistențăGuid / sourceComportamentul anchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705745"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b3cad-102">ConsistențăGuid / sourceComportamentul anchor</span><span class="sxs-lookup"><span data-stu-id="b3cad-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b3cad-103">Azure AD conecta (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="b3cad-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b3cad-104">Când utilizați această caracteristică, Azure AD conecta configurează automat regulile de sincronizare la:</span><span class="sxs-lookup"><span data-stu-id="b3cad-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b3cad-105">Utilizați msDS-ConsistyGuid ca atribut sourceAnchor pentru obiecte de utilizator.</span><span class="sxs-lookup"><span data-stu-id="b3cad-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b3cad-106">ObjectGUID este utilizat pentru alte tipuri de obiecte.</span><span class="sxs-lookup"><span data-stu-id="b3cad-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b3cad-107">Pentru orice obiect dat local de utilizator AD al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect scrie valoarea objectGUID înapoi la atributul msDS-ConsistencyGuid în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="b3cad-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b3cad-108">După ce atributul msDS-ConsistyGuid este populat, Azure AD conecta apoi exportă obiectul azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3cad-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b3cad-109">**Notã:** Odată ce un obiect AD local este importat în Azure AD Connect (adică, importatîn spațiul de conector AD și proiectat în Metaverse), nu se poate modifica valoarea sourceAnchor mai.</span><span class="sxs-lookup"><span data-stu-id="b3cad-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b3cad-110">Pentru a specifica valoarea sourceAnchor pentru un obiect AD local dat, configurați atributul msDS-ConsistyGuid înainte de a fi importat în Azure AD conecta.</span><span class="sxs-lookup"><span data-stu-id="b3cad-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b3cad-111">Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [Azure AD conecta: concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b3cad-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

