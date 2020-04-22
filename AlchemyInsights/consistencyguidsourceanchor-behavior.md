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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistențăGuid / sourceComportamentul anchor

Azure AD conecta (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca atribut sourceAnchor. Când utilizați această caracteristică, Azure AD conecta configurează automat regulile de sincronizare la:
  
- Utilizați msDS-ConsistyGuid ca atribut sourceAnchor pentru obiecte de utilizator. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice obiect dat local de utilizator AD al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect scrie valoarea objectGUID înapoi la atributul msDS-ConsistencyGuid în Active Directory local. După ce atributul msDS-ConsistyGuid este populat, Azure AD conecta apoi exportă obiectul azure AD.
    
 **Notã:** Odată ce un obiect AD local este importat în Azure AD Connect (adică, importatîn spațiul de conector AD și proiectat în Metaverse), nu se poate modifica valoarea sourceAnchor mai. Pentru a specifica valoarea sourceAnchor pentru un obiect AD local dat, configurați atributul msDS-ConsistyGuid înainte de a fi importat în Azure AD conecta. 
  
Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [Azure AD conecta: concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

