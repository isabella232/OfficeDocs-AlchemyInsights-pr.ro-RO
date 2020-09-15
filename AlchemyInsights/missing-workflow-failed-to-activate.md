---
title: Fluxul de lucru lipsă nu a putut fi activat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667098"
---
# <a name="missing-workflow-failed-to-activate"></a>Fluxul de lucru lipsă nu a putut fi activat

Într-o colecție de site-uri Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil global (cum ar fi "aprobare-SharePoint 2010") într-o listă sau o bibliotecă.
  
Pentru a rezolva această problemă, urmați acești pași: 
  
1. Deschideți site-ul web rădăcină al colecției de site-uri în SharePoint Designer 2013.
  
2. Sub **obiecte site**, selectați **fluxuri de lucru**. 
  
3. În secțiunea **nouă** a panglicii **fluxuri de lucru** , selectați **flux de lucru reutilizabil**. 
  
4. În formularul **Creați un flux de lucru reutilizabil** , introduceți numele * * *Repair2010* * *. Pentru **tip platformă**, faceți clic pe **flux de lucru SharePoint 2010**, apoi faceți clic pe **OK**. 
  
1. În secțiunea **Salvare** a panglicii **fluxului de lucru** , selectați **Publicare**. 
  
2. În secțiunea **gestionare** a panglicii **fluxului de lucru** , selectați **Publicare la nivel global**. În caseta de dialog de confirmare care apare, selectați **OK**. 
  
3. Într-un browser web, găsiți site-ul web rădăcină al colecției de site **Site Settings** -uri, apoi accesați \> **caracteristicile colecției**site-ului setări site. Apoi, comutați caracteristica **fluxuri de lucru** : 
  
· Dacă caracteristica este  *activată*  , faceți clic pe Dezactivare **,** apoi faceți clic pe **Activare**. 
  
· Dacă caracteristica este  *dezactivată*  , faceți clic pe **Activare**. 
  
Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

