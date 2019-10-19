---
title: Flux de lucru lipsă nu a reușit să activați
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753808"
---
# <a name="missing-workflow-failed-to-activate"></a>Flux de lucru lipsă nu a reușit să activați

Într-o colecție de site-ul Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabile global (cum ar fi "aprobare-SharePoint 2010") la o listă sau bibliotecă.
  
Pentru a rezolva această problemă, urmați acești pași: 
  
1. Deschideți site-ul rădăcină al colecția de site-uri în SharePoint Designer 2013.
  
2. Sub **obiecte site**, selectați **fluxuri**de lucru. 
  
3. În secțiunea **nouă** a panglicii **fluxurilor** de lucru, selectați **flux de lucru reutilizabile**. 
  
4. În formularul **Creare flux de lucru reutilizabile** , introduceți numele * * *Repair2010* * *. Pentru **tip de platformă**, faceți clic pe **SharePoint 2010 flux de lucru**, și apoi faceți clic pe **OK**. 
  
1. În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**. 
  
2. În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare globală**. În caseta de dialog de confirmare care apare, selectați **OK**. 
  
3. Într-un browser web, localizați site-ul web rădăcină al colecției de site-uri, apoi accesați **caracteristicile de colecție**site-ul de **Setări** \> site. Apoi, comutați caracteristica **fluxuri** de lucru: 
  
· Dacă caracteristica este *activată* , faceți clic pe **Dezactivare,** apoi faceți clic pe **Activare**. 
  
· Dacă caracteristica este *dezactivată* , faceți clic pe **Activare**. 
  
Pentru mai multe informații vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

