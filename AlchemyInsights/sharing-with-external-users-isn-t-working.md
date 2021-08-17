---
title: Partajarea cu utilizatorii externi nu funcționează
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304381"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Remedierea problemelor cu SharePoint conținut cu utilizatorii externi

Asigurați-vă că este activată partajarea externă pentru organizația dvs.:
  
1. Accesați pagina Programe de completare servicii din pagina de Centru de administrare Microsoft 365 și [ &amp; faceți](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)clic pe **Site-uri.**
    
2. Asigurați-vă că setarea este activată la "Activat". Dacă este selectat "Doar utilizatorii externi existenți", asigurați-vă că utilizatorul extern este listat în lista Centru de administrare Microsoft 365.
    
Asigurați-vă că a fost activată partajarea externă pentru site. Pentru o colecție de site-uri clasică:
  
1. În noul centru de administrare SharePoint, în panoul din stânga, faceți clic pe **Site-uri**.
    
2. Selectați site-ul sau site-urile și, pe panglică, faceți clic **pe Partajare.**
    
Pentru un site de echipă care aparține unui Microsoft 365 grup de comunicații sau unui site de comunicare:
  
- Aceste noi tipuri de site-uri au aceeași setare de partajare ca setarea la nivel de organizație, cu excepția cazului în care setarea la nivel de organizație permite partajarea fișierelor utilizând linkuri care nu necesită conectare. În acest caz, site-urile permit partajarea cu utilizatori externi noi și existenți care se autentifică. Pentru a modifica setarea pentru anumite site-uri, utilizați noul centru SharePoint sau PowerShell. [Aflați mai multe](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Notă:** setarea de partajare externă pentru orice site poate fi mai restrictivă decât setarea la nivel de organizație, dar nu mai permisivă decât setarea la nivel de organizație. 
  

