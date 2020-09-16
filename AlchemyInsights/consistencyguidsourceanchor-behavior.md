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
# <a name="consistencyguid--sourceanchor-behavior"></a>Comportamentul ConsistencyGuid/sourceAnchor

Azure AD Connect (versiunea 1.1.524.0 și After) facilitează acum utilizarea AMS-ConsistencyGuid ca atribut sourceAnchor. Atunci când utilizați această caracteristică, Azure AD Connect configurează automat regulile de sincronizare pentru:
  
- Utilizați AMS-ConsistencyGuid ca atribut sourceAnchor pentru obiectele de utilizator. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice obiect de utilizator de publicitate local al cărui atribut AMS-ConsistencyGuid nu este populat, Azure AD Connect își scrie valoarea objectGUID înapoi la atributul AMS-ConsistencyGuid în Active Directory local. După ce atributul AMS-ConsistencyGuid este populat, Azure AD Connect exportă obiectul la Azure AD.
    
 **Notă:** După ce un obiect de publicitate local este importat în Azure AD Connect (adică importat în spațiul conectorului de publicitate și proiectat în metaverse), nu mai puteți modifica valoarea sa sourceAnchor. Pentru a specifica valoarea sourceAnchor pentru un anumit obiect de publicitate local, configurați atributul său AMS-ConsistencyGuid înainte de a fi importat în Azure AD Connect. 
  
Pentru mai multe informații despre SourceAnchor și ConsistencyGuid, consultați următoarele: [AZURE AD Connect: concepte de proiectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

