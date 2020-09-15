---
title: Eroare AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709163"
---
# <a name="error-attributevaluemustbeunique"></a>Eroare: AttributeValueMustBeUnique

Motivul cel mai comun pentru eroarea AttributeValueMustBeUnique este că două obiecte cu SourceAnchor diferite (immutableId) au aceeași valoare pentru atributele ProxyAddresses și/sau UserPrincipalName. Pentru a remedia eroarea AttributeValueMustBeUnique:
  
1. Identificați valoarea de atribut proxyAddresses, userPrincipalName sau alt atribut care cauzează eroarea. De asemenea, identificați care două (sau mai multe) obiecte sunt implicate în conflict. Raportul generat de Azure AD Connect Health pentru sincronizare vă poate ajuta să identificați cele două obiecte.
    
2. Identificați obiectul care ar trebui să continue să aibă valoarea dublată și obiectul care nu ar trebui să fie.
    
3. Eliminați valoarea dublată din obiectul care nu ar trebui să aibă acea valoare. Rețineți că trebuie să efectuați modificarea în directorul din care provine obiectul. În unele cazuri, poate fi necesar să ștergeți unul dintre obiectele din conflict.
    
4. Dacă ați efectuat modificarea în ANUNȚul local, permiteți ca Azure AD Connect să sincronizeze modificarea erorii pentru a fi remediată.
    

