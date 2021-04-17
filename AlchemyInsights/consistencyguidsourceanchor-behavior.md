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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistențăGuid /sourceAnchor behavior

Azure AD Connect (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca atribut sourceAnchor. Atunci când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare la:
  
- Utilizați msDS-ConsistencyGuid ca atribut sourceAnchor pentru obiectele User. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice obiect AD User local dat al cărui atribut msDS-ConsistencyGuid nu este populat, Azure AD Connect își scrie valoarea objectGUID înapoi în atributul msDS-ConsistencyGuid în Active Directory local. După ce este populat atributul msDS-ConsistencyGuid, Azure AD Connect exportă apoi obiectul în Azure AD.
    
 **Notă:** După ce un obiect AD local este importat în Azure AD Connect (care este importat în Spațiul conectorului AD și proiectat în Metaversu), nu îi mai puteți modifica valoarea sourceAnchor. Pentru a specifica valoarea sourceAnchor pentru un anumit obiect AD local, configurați atributul msDS-ConsistencyGuid înainte ca acesta să fie importat în Azure AD Connect. 
  
Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [Azure AD Connect: Concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

