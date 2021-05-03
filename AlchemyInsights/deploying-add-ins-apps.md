---
title: Implementarea programelor de completare pentru Aplicații Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125683"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Implementarea programelor de completare pentru Aplicații Microsoft 365

Implementarea centralizată este modul recomandat pentru implementarea Office de completare pentru utilizatori și grupuri în cadrul organizației. Pentru a implementa programe de completare, urmați pașii de mai jos:

**Notă:** Pentru a instala programe de completare pentru Office ca utilizator individual, consultați Vizualizarea, gestionarea și instalarea programelor de [completare Office programele.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) De asemenea, asigurați-vă că achiziționarea individuală de Office de completare din Magazin este activată. 

1. Asigurați-vă că mediul dvs. îndeplinește cerințele pentru implementarea de programe de completare care utilizează Implementarea centralizată. Pentru detalii, consultați [Cerințe.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Accesați Pagina **Setări Aplicații**  >  **integrate**  >  **Obțineți aplicații din** centrul Microsoft 365 administrare pentru a implementa programe de completare. 

Note: 

- Aplicațiile integrate necesită ca administratorul să dea permisiuni de Administrator global Exchange permisiuni de Administrator.

- Atunci când implementați programe de completare pentru mai mulți utilizatori, vă recomandăm să atribuiți utilizând grupuri în loc de utilizatori individuali. Pentru detalii, consultați [Considerații atunci când atribuiți un program de completare utilizatorilor și grupurilor.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Implementarea centralizată nu acceptă utilizatorii din grupuri imbricate sau grupuri care au grupuri părinte. Pentru detalii, consultați [Atribuirile de utilizator și de grup.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Asigurați-vă că serviciul Microsoft 365 de gestionare a aplicațiilor (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') este activat pentru ca utilizatorii să se conecteze. Pentru detalii, consultați Configurarea [proprietăților aplicațiilor.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Dacă vă experimentați probleme la implementarea programelor de completare utilizând aplicații integrate, încercați să implementați [utilizând programe de completare.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Pentru mai multe informații, consultați:

[Implementarea de programe de completare în centrul de administrare](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gestionarea programelor de completare în centrul de administrare](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizarea cmdletelor PowerShell de implementare centralizată pentru a gestiona programe de completare](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicarea Office completare utilizând Implementarea centralizată prin centrul Microsoft 365 administrare](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Depanare: Utilizatorul nu vede programele de completare](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Depanarea erorilor utilizatorilor cu Office de completare](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)