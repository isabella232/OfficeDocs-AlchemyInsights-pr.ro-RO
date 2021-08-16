---
title: Fluxul de lucru lipsă nu a reușit activarea
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065440"
---
# <a name="missing-workflow-failed-to-activate"></a>Fluxul de lucru lipsă nu a reușit activarea

Într-o colecție de site-SharePoint Microsoft SharePoint, nu puteți adăuga un flux de lucru reutilizabil global (cum ar fi "Aprobare - SharePoint 2010") la o listă sau la o bibliotecă.
  
Pentru a rezolva această problemă, urmați acești pași: 
  
1. Deschideți site-ul web rădăcină al colecției de site-uri SharePoint Designer 2013.
  
2. Sub Obiecte **site,** selectați **Fluxuri de lucru.** 
  
3. În secțiunea **Nou** a panglicii **Fluxuri de lucru,** selectați **Flux de lucru reutilizabil.** 
  
4. Pe formularul **Creare flux de lucru reutilizabil,** introduceți numele ** *Reparare2010* **. Pentru **Tip platformă ,** faceți clic SharePoint **2010 Workflow**, apoi faceți clic pe **OK.** 
  
1. În secțiunea **Salvare** a panglicii **Flux de lucru,** selectați **Publicare**. 
  
2. În **secțiunea Gestionare** din panglica **Flux de** lucru, **selectați Publicare globală.** În caseta de dialog de confirmare care apare, selectați **OK.** 
  
3. Într-un browser web, găsiți site-ul web rădăcină al colecției de site-uri, apoi **accesați Site Setări Caracteristici** colecție de \> **site-uri.** Apoi comutați caracteristica Fluxuri **de lucru:** 
  
· Dacă această caracteristică este *Activată,* **faceți clic pe Dezactivare, apoi** pe **Activare.** 
  
· În cazul în care caracteristica este  *dezactivată, faceți*  clic **pe Activare**. 
  
Pentru mai multe informații, consultați articolul [următor.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

