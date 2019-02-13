---
title: Sharing cu utilizatorii externi nu este de lucru
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900895"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Remediați problemele conținut SharePoint de partajare cu utilizatorii externi

Asiguraţi-vă că partajarea externă este activată pentru organizaţie:
  
1. Du-te la [servicii &amp; pagina de completare în centrul de administrare Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), faceţi clic pe **site-uri**.
    
2. Asiguraţi-vă că setarea este apelat la "Pe". Dacă este selectat "Doar utilizatorii existenţi externe", asiguraţi-vă că utilizatorul extern este listat în centrul de administrare Office 365.
    
Asiguraţi-vă că extern de partajare-l activat pentru site-ul. Pentru o colecţie de site-ul clasic:
  
1. În centrul de administrare SharePoint clasic, în panoul din stânga, faceţi clic pe **site-ul colecţii**.
    
2. Selectaţi site-ul sau site-uri, şi panglică, faceţi clic pe **Partajare**.
    
Pentru un site de echipă, care aparţine unui grup de Office 365, sau un site de comunicare:
  
- Aceste tipuri de site-ul nou au setarea partajare aceeaşi ca setarea de nivel de organizaţie, dacă setarea de nivel de organizaţie permite partajarea fişierelor folosind link-uri care nu necesită autentificare. În acest caz, site-uri permite partajarea cu noi și existente de utilizatori externi care semnează în. Pentru a modifica setarea pentru anumite site-uri, utilizaţi noul centru de administrare SharePoint (preview) sau PowerShell. [Aflaţi mai multe](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Setarea de partajare externă pentru orice site poate fi mai restrictive decât setarea de nivel de organizaţie, dar nu mai permisivă decât setarea de nivel de organizaţie. 
  

