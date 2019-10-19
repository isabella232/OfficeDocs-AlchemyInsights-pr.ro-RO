---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502243"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Remedierea problemelor cu partajarea conținutului SharePoint cu utilizatorii externi

Asigurați-vă că partajarea externă este activată pentru organizația dvs.:
  
1. Accesați pagina de [ &amp; programe de completare din centrul de administrare Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)și faceți clic pe **site-uri**.
    
2. Asigurați-vă că setarea este activată "activat". Dacă este selectată "numai utilizatorii externi existenți", asigurați-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.
    
Asigurați-vă că partajarea externă este activată pentru site. Pentru o colecție de site-uri clasice:
  
1. În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **site-uri**.
    
2. Selectați site-ul sau site-urile și, în panglică, faceți clic pe **Partajare**.
    
Pentru un site de echipă care aparține unui grup Office 365 sau un site de comunicare:
  
- Aceste tipuri de site-uri noi au aceeași setare de partajare ca setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare. În acest caz, site-urile permit partajarea cu utilizatori externi noi și existenți care se conectează. Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru de administrare SharePoint sau PowerShell. [Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație. 
  

