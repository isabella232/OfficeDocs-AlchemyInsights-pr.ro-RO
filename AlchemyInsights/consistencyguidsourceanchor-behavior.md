---
title: ConsistencyGuid / sourceAnchor de comportament
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659603"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor de comportament

Azur AD Connect (versiunea 1.1.524.0 şi după) acum facilitează utilizarea ConsistencyGuid AMS ca atributul sourceAnchor. Atunci când se utilizează această caracteristică, Azure AD conecta configurează automat regulile sincronizare:
  
- Utilizarea ConsistencyGuid AMS ca atributul sourceAnchor pentru obiectele utilizator. ObjectGUID este utilizat pentru alte tipuri de obiecte.
    
- Pentru orice dat local AD utilizator obiect a cărui atribut de AMS-ConsistencyGuid nu este populat, Azure AD conecta scrie valoarea objectGUID înapoi la atributul de AMS-ConsistencyGuid în Active Directory local. După atributul AMS-ConsistencyGuid este populat, Azure AD conecta apoi exportă obiectul azuriu AD.
    
 **Notă:** O dată un local AD obiect este importat în Azure AD conecta (adică, importate în spaţiul conector AD şi proiectat în Metaverse), nu se poate modifica valoarea sa sourceAnchor mai. Pentru a preciza valoarea sourceAnchor o dat local AD obiect, configuraţi atributul lui AMS-ConsistencyGuid înainte de a acesta este importat în Azure AD Connect. 
  
Pentru mai multe informaţii despre SourceAnchor şi ConsistencyGuid, se referă la următoarele: [Azure AD conecta: concepte de Design](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

