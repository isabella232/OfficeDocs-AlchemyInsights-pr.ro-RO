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
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamentul ConsistencyGuid/sourceAnchor

Azure AD Connect (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca sourceAnchor atribut. Când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare la:
  
- Utilizați msDS-ConsistencyGuid ca atributul sourceAnchor pentru obiectele de utilizator. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice anumit obiect de utilizator AD local al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect scrie valoarea objectGUID înapoi la atributul msDS-ConsistencyGuid în Active Directory local. După atributul msDS-ConsistencyGuid este populat, Azure AD Connect apoi exportă obiectul Azure AD.
    
 **Notă:** Odată ce un obiect AD local este importat în Azure AD Connect (care este, importate în spațiul de conector AD și proiectate în metaverse), nu se poate modifica valoarea sourceAnchor mai. Pentru a specifica valoarea sourceAnchor pentru un anumit obiect AD local, configurați atributul msDS-ConsistencyGuid înainte de a fi importate în Azure AD Connect. 
  
Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [AZURE AD Connect: concepte de design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

