---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813772"
---
# <a name="error-attributevaluemustbeunique"></a>Eroare: AttributeValueMustBeUnique

Motivul cel mai comun al erorii AttributeValueMustBeUnique este că două obiecte cu sourceAnchor diferit (inutilizabilId) au aceeași valoare pentru atributele ProxyAddresses și/sau UserPrincipalName. Pentru a remedia eroarea AttributeValueMustBeUnique:
  
1. Identificați adresa proxyAddresses dublată, userPrincipalName sau altă valoare de atribut care provoacă eroarea. Identificați și ce două (sau mai multe) obiecte sunt implicate în conflict. Raportul generat de Azure AD Connect Health pentru sincronizare vă poate ajuta să identificați cele două obiecte.
    
2. Identificați ce obiect trebuie să continue să aibă valoarea dublată și ce obiect nu trebuie să aibă.
    
3. Eliminați valoarea dublată din obiectul care NU trebuie să aibă acea valoare. Rețineți că trebuie să efectuați modificarea în directorul din care provine obiectul. În unele cazuri, poate fi necesar să ștergeți unul dintre obiectele care intră în conflict.
    
4. Dacă faceți modificarea în AD local, permiteți ca Azure AD Connect să sincronizeze modificarea pentru ca eroarea să fie remediată.
    

