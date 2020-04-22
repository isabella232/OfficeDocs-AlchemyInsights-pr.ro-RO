---
title: Fluxul de lucru lipsă nu a reușit să se activeze
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762113"
---
# <a name="missing-workflow-failed-to-activate"></a>Fluxul de lucru lipsă nu a reușit să se activeze

Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "Aprobare - SharePoint 2010") la o listă sau la o bibliotecă.
  
Pentru a rezolva această problemă, urmați acești pași: 
  
1. Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.
  
2. Sub **Obiecte site**, selectați Fluxuri de **lucru**. 
  
3. În secțiunea **Nou** din panglica **Fluxuri de lucru,** selectați **Flux de lucru reutilizabil**. 
  
4. În formularul **Creare flux de lucru reutilizabil,** introduceți numele ** *Repair2010* **. Pentru **Platformă Tip**, faceți clic pe **Flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**. 
  
1. În secțiunea **Salvare** din panglica **Flux de lucru,** selectați **Publicare**. 
  
2. În secțiunea **Gestionare** din panglica Flux de **lucru,** selectați **Publicare globală**. În caseta de dialog de confirmare care apare, selectați **OK**. 
  
3. Într-un browser web, găsiți site-ul web rădăcină al colecției de site-uri, apoi accesați **Caracteristici colecție de site-uri** **setări** \> site. Apoi, comutați caracteristica **Fluxuri de lucru:** 
  
· Dacă caracteristica este *Activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**. 
  
· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**. 
  
Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

