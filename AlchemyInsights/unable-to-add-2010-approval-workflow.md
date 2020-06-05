---
title: Imposibil de adăugat fluxul de lucru de aprobare 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582859"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Imposibil de adăugat fluxul de lucru de aprobare 2010

Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "Aprobare - SharePoint 2010") la o listă sau la o bibliotecă.
  
Pentru a rezolva această problemă, urmați acești pași: 
  
1. Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.
  
2. Sub **Obiecte site**, selectați Fluxuri de **lucru**. 
  
3. În secțiunea **Nou** din panglica **Fluxuri de lucru,** selectați **Flux de lucru reutilizabil**. 
  
4. În formularul **Creare flux de lucru reutilizabil,** introduceți numele ** *Repair2010* **. Pentru **Platformă Tip**, faceți clic pe **Flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**. 
  
1. În secțiunea **Salvare** din panglica **Flux de lucru,** selectați **Publicare**. 
  
2. În secțiunea **Gestionare** din panglica Flux de **lucru,** selectați **Publicare globală**. În caseta de dialog de confirmare care apare, selectați **OK**. 
  
3. Într-un browser web, găsiți site-ul web rădăcină al colecției de site-uri, apoi accesați Caracteristici colecție de **Site Settings** \> **site-uri**setări site. Comutați caracteristica **Fluxuri de lucru:** 
  
· Dacă caracteristica este *Activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**. 
  
· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**. 
  
Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

