---
title: Deschiderea cu Explorer nu funcționează
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713046"
---
# <a name="open-with-explorer-isnt-working"></a>Deschiderea cu Explorer nu funcționează

Dacă **Deschidere cu Explorer** sau Vizualizare în **Explorer** nu funcționează, asigurați-vă că serviciul WebClient este setat la **Executare** urmând pașii de mai jos. De exemplu, poate dura mult timp pentru a deschide o bibliotecă SharePoint sau OneDrive atunci când serviciul nu se execută. 
  
1. În caseta de căutare Windows, tastați executare, selectați aplicația Executare desktop, tastați services.msc, apoi **selectați Enter**.
    
2. Defilați în jos la serviciul WebClient și verificați coloana **Stare.** Dacă starea serviciului WebClient nu **se execută**, faceți dublu clic pe serviciu, faceți clic pe **Start**, apoi faceți clic pe **OK**. Activați serviciul, dacă este necesar, selectând **Manual** sau **Automat** în caseta **Tip pornire.** 
    
> [!NOTE]
> Pentru a depana problemele de deschidere în Explorer, consultați [Deschiderea în Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explorați sincronizarea ca alternativă mai bună: [sincronizați fișierele SharePoint cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

