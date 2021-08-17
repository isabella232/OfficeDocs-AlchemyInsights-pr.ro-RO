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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044352"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistențăGuid /sourceAnchor behavior

Azure AD Conectare (versiunea 1.1.524.0 și după) facilitează acum utilizarea msDS-ConsistencyGuid ca atribut sourceAnchor. Atunci când utilizați această caracteristică, Azure AD Conectare configurează automat regulile de sincronizare pentru:
  
- Utilizați msDS-ConsistencyGuid ca atribut sourceAnchor pentru obiectele User. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice obiect AD Utilizator local dat al cărui atribut msDS-ConsistGuid nu este populat, Azure AD Conectare își scrie valoarea objectGUID înapoi în atributul msDS-ConsistencyGuid în Active Directory local. După ce este populat atributul msDS-ConsistencyGuid, Azure AD Conectare apoi exportă obiectul în Azure AD.
    
 **Notă:** Odată ce un obiect AD local este importat în Azure AD Conectare (care este importat în Spațiul conectorului AD și proiectat în Metaverse), nu-i mai puteți modifica valoarea sourceAnchor. Pentru a specifica valoarea sourceAnchor pentru un anumit obiect AD local, configurați atributul msDS-ConsistencyGuid înainte ca acesta să fie importat în Azure AD Conectare. 
  
Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [Azure AD Conectare: Concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

