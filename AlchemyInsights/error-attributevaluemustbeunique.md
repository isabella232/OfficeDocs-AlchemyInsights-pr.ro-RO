---
title: Eroare AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703186"
---
# <a name="error-attributevaluemustbeunique"></a>Eroare: AttributeValueMustBeUnique

Cel mai frecvent motiv pentru eroarea AttributeValueMustBeUnique este două obiecte cu SourceAnchor diferite (immutableId) au aceeași valoare pentru atributele ProxyAddresses și/sau UserPrincipalName. Pentru a remedia eroarea AttributeValueMustBeUnique:
  
1. Identificați proxyAddresses dublate, userPrincipalName sau altă valoare de atribut care provoacă eroarea. De asemenea, identificați care două (sau mai multe) obiecte sunt implicate în conflict. Raportul generat de Azure AD Connect Sănătate pentru sincronizare vă poate ajuta să identificați cele două obiecte.
    
2. Identificați obiectul care ar trebui să continue să aibă valoarea dublată și ce obiect nu ar trebui.
    
3. Eliminați valoarea dublată din obiectul care nu ar trebui să aibă această valoare. Rețineți că trebuie să efectuați modificarea în directorul din care provine obiectul. În unele cazuri, poate fi necesar să ștergeți unul dintre obiectele aflate în conflict.
    
4. Dacă ați făcut modificarea în local AD, permiteți Azure AD Connect sincroniza modificarea pentru eroarea pentru a obține remediate.
    

