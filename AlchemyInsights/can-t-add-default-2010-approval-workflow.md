---
title: Imposibil de adăugat implicit fluxul de lucru aprobare 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306558"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Imposibil de adăugat implicit fluxul de lucru aprobare 2010

Într-o colecţie de site-ul Microsoft SharePoint, nu puteţi adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "aprobare - SharePoint 2010") o listă sau o bibliotecă.
  
Pentru a rezolva această problemă, urmaţi aceşti paşi: 
  
1. Deschide site-ul rădăcină din colecția de site-ul în SharePoint Designer 2013.
  
2. Cu **Site-ul obiectele**, selectați **fluxuri de lucru**. 
  
3. În secţiunea **noua** de panglica de **fluxuri de lucru** , selectaţi **Flux de lucru reutilizabil**. 
  
4. Formular **Creare flux de lucru reutilizabil** , introduceţi numele * **Repair2010***. Pentru **Platforma de tip**, selectaţi **Flux de lucru SharePoint 2010**, şi apoi selectaţi **OK**. 
  
5. În secţiunea **Salvare** de panglica de **flux de lucru** , selectaţi **Publicare**. 
  
6. În secţiunea de **administrare** a panglicii de **flux de lucru** , selectaţi **Publica la nivel global**. În casetă de dialog de confirmare care apare, selectaţi **OK**. 
  
7. Într-un browser web, localizați site-ul rădăcină al colecției de site-uri, şi apoi accesa **Site-ul setările** \> **Caracteristici de colectare site-ului**. Apoi, comuta caracteristica de **fluxuri de lucru** : 
  
· În cazul în care funcţia este *activ* , faceţi clic pe **Dezactivare,** şi apoi faceţi clic pe **Activare**. 
  
· În cazul în care funcţia este *dezactivata* , faceţi clic pe **Activare**. 
  
Pentru mai multe informaţii vă rugăm să consultaţi următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

