---
title: Eroare Atributevaluemustbeunique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36527043"
---
# <a name="error-attributevaluemustbeunique"></a>Eroare: AttributeValueMustBeUnique

Cel mai frecvent motiv pentru eroarea AttributeValueMustBeUnique este două obiecte cu SourceAnchor diferite (immutableId) au aceeași valoare pentru atributele ProxyAddresses și/sau UserPrincipalName. Pentru a remedia eroarea AttributeValueMustBeUnique:
  
1. Identificați proxyAddresses duplicate, userPrincipalName sau altă valoare de atribut care cauzează eroarea. De asemenea, identificați care două (sau mai multe) obiecte sunt implicate în conflict. Raportul generat de Azure AD Connect Health pentru sincronizare vă poate ajuta să identificați cele două obiecte.
    
2. Identificați care obiect ar trebui să continue să aibă valoarea duplicată și care obiectul nu ar trebui să.
    
3. Eliminați valoarea duplicată din obiectul care nu ar trebui să aibă această valoare. Rețineți că ar trebui să efectuați modificarea în directorul de unde provine obiectul. În unele cazuri, poate fi necesar să ștergeți unul dintre obiectele din conflict.
    
4. Dacă ați făcut modificarea în local AD, permiteți Azure AD Connect sincroniza modificarea pentru eroarea pentru a obține fix.
    

