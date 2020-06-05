---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582787"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Remedierea problemelor legate de partajarea conținutului SharePoint cu utilizatorii externi

Asigurați-vă că partajarea externă este activată pentru organizația dvs.:
  
1. Accesați [pagina Programe de completare Servicii din centrul de administrare Microsoft &amp; 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)și faceți clic pe **Site-uri**.
    
2. Asigurați-vă că setarea este activată la "Activat". Dacă este selectată opțiunea "Numai utilizatorii externi existenți", asigurați-vă că utilizatorul extern este listat în centrul de administrare Microsoft 365.
    
Asigurați-vă că partajarea externă activată pentru site. Pentru o colecție clasică de site-uri:
  
1. În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **site-uri**.
    
2. Selectați site-ul sau site-urile, iar pe panglică, faceți clic pe **Partajare**.
    
Pentru un site de echipă care aparține unui grup Microsoft 365 sau unui site de comunicare:
  
- Aceste tipuri noi de site-uri au aceeași setare de partajare ca și setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare. În acest caz, site-urile permit partajarea cu utilizatorii externi noi și existenți care se conectează. Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru de administrare SharePoint sau PowerShell. [Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație. 
  

