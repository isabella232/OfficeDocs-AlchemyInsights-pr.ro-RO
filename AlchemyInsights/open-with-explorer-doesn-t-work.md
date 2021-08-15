---
title: Deschiderea cu Explorer nu funcționează
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011348"
---
# <a name="open-with-explorer-isnt-working"></a>Deschiderea cu Explorer nu funcționează

Dacă **Deschidere cu Explorer** sau Vizualizare în **Explorer** nu funcționează, asigurați-vă  că serviciul WebClient este setat la Executare urmând pașii de mai jos. De exemplu, poate dura mult timp să deschideți o bibliotecă SharePoint sau OneDrive atunci când serviciul nu rulează. 
  
1. În caseta Windows căutare, tastați **executare,** selectați Executare aplicație desktop, tastați services.msc, apoi selectați Enter .
    
2. Defilați în jos la serviciul WebClient și verificați **coloana** Stare. Dacă starea serviciului WebClient nu rulează **,** faceți dublu clic pe serviciu, faceți **clic pe Start**, apoi pe **OK**. Activați serviciul, dacă este necesar, selectând **Manual** sau **Automat** în **caseta Tip pornire.** 
    
> [!NOTE]
> Pentru a depana problemele de deschidere în Explorer, [consultați Deschidere în Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Explorați sincronizarea ca alternativă mai [bună: SharePoint cu noul client Sincronizare cu OneDrive sincronizare](https://go.microsoft.com/fwlink/?linkid=871666). 
  

