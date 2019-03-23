---
title: Deschidere cu Explorer nu funcţionează
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764920"
---
# <a name="open-with-explorer-isnt-working"></a>Deschidere cu Explorer nu este de lucru

În cazul în care nu funcţionează **Deschidere cu Explorer** sau **din File Explorer** asiguraţi-vă că serviciul WebClient este setat să **ruleze** urmând paşii de mai jos. De exemplu, ar putea dura mult timp pentru a deschide o bibliotecă SharePoint sau OneDrive, atunci când acest serviciu nu se execută. 
  
1. În caseta de căutare Windows, tip alerga, selectaţi app desktop a alerga, tip services.msc, şi apoi selectaţi **Enter**.
    
2. Derulaţi în jos la serviciu WebClient şi verificaţi coloana de **stare** . În cazul în care starea de service WebClient nu este **rulează**, faceţi dublu clic pe servicii, faceţi clic pe **Start**şi apoi faceţi clic pe **OK**. Activarea serviciului, dacă este necesar, selectând fie **Manual** , fie **automat** în caseta de **tip Startup** . 
    
> [!NOTE]
> Pentru a depana probleme de deschidere în File Explorer, consultaţi [deschis în Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explora sincronizare ca o alternativă mai bună: [SharePoint sincronizare fişiere cu noul client de sincronizare OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

