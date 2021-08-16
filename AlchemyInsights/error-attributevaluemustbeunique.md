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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002132"
---
# <a name="error-attributevaluemustbeunique"></a>Eroare: AttributeValueMustBeUnique

Motivul cel mai comun al erorii AttributeValueMustBeUnique este că două obiecte cu sourceAnchor diferit (inutilizabilId) au aceeași valoare pentru atributele ProxyAddresses și/sau UserPrincipalName. Pentru a remedia eroarea AttributeValueMustBeUnique:
  
1. Identificați adresa proxyAddresses dublată, userPrincipalName sau altă valoare de atribut care provoacă eroarea. Identificați și ce două (sau mai multe) obiecte sunt implicate în conflict. Raportul generat de Azure AD Conectare Starea sincronizării vă poate ajuta să identificați cele două obiecte.
    
2. Identificați ce obiect trebuie să continue să aibă valoarea dublată și ce obiect nu trebuie să aibă.
    
3. Eliminați valoarea dublată din obiectul care NU trebuie să aibă acea valoare. Rețineți că trebuie să efectuați modificarea în directorul din care provine obiectul. În unele cazuri, poate fi necesar să ștergeți unul dintre obiectele care intră în conflict.
    
4. Dacă faceți modificarea în AD local, permiteți ca Azure AD Conectare sincronizeze modificarea pentru ca eroarea să fie remediată.
    

