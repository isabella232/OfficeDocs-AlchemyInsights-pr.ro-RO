---
title: Lipsă de flux de lucru nu a reuşit pentru a activa
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543937"
---
# <a name="missing-workflow-failed-to-activate"></a>Lipsă de flux de lucru nu a reuşit pentru a activa

Într-o colecţie de site-ul Microsoft SharePoint, nu puteţi adăuga un flux de lucru reutilizabil la nivel global (cum ar fi "aprobare - SharePoint 2010") o listă sau o bibliotecă.
  
Pentru a rezolva această problemă, urmaţi aceşti paşi: 
  
1. Deschide site-ul rădăcină din colecția de site-ul în SharePoint Designer 2013.
  
2. Cu **Site-ul obiectele**, selectați **fluxuri de lucru**. 
  
3. În secţiunea **noua** de panglica de **fluxuri de lucru** , selectaţi **Flux de lucru reutilizabil**. 
  
4. Formular **Creare flux de lucru reutilizabil** , introduceţi numele ** *Repair2010* **. Pentru **Platforma de tip**, faceţi clic pe **Flux de lucru SharePoint 2010**, şi apoi faceţi clic pe **OK**. 
  
1. În secţiunea **Salvare** de panglica de **flux de lucru** , selectaţi **Publicare**. 
  
2. În secţiunea de **administrare** a panglicii de **flux de lucru** , selectaţi **Publica la nivel global**. În casetă de dialog de confirmare care apare, selectaţi **OK**. 
  
3. Într-un browser web, localizați site-ul rădăcină al colecției de site-uri, şi apoi accesa **Site-ul setările** \> **Caracteristici de colectare site-ului**. Apoi, comuta caracteristica de **fluxuri de lucru** : 
  
· În cazul în care funcţia este *activ* , faceţi clic pe **Dezactivare,** şi apoi faceţi clic pe **Activare**. 
  
· În cazul în care funcţia este *dezactivata* , faceţi clic pe **Activare**. 
  
Pentru mai multe informaţii vă rugăm să consultaţi următorul [articol](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

