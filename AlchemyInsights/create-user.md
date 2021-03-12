---
title: Creați un utilizator
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747024"
---
# <a name="create-user"></a>Creați un utilizator

**ANUNȚ**

- [Dezaprobarea suportului de conectare pentru vizualizare de la Google începând cu 4 ianuarie 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Testați dacă aplicațiile dumneavoastră pot fi afectate, urmând [instrucțiunile Google](https://go.microsoft.com/fwlink/?linkid=2157323) privind compatibilitatea testării.
- Asigurați-vă că utilizați vizualizarea web sau browserul de sistem la conectarea utilizatorilor cu conturi Google pentru consumatori. Pentru mai multe informații, consultați [probleme la conectarea la aplicații utilizând doar browserul Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Nu pot crea un utilizator nou în directorul Azure AD**

1. Asigurați-vă că sunteți autorizat să creați un nou utilizator standard. Doar rolul administratorului general sau al administratorului de utilizator din Azure Active Directory (AD) poate crea un nou utilizator standard. Dacă nu sunteți într-unul dintre aceste roluri, solicitați unui administrator să vă adauge la unul dintre aceste roluri sau să vă creeze noul cont de utilizator.
1. Asigurați-vă că numele de utilizator se află într-un domeniu care este verificat în reclama Azure. Dacă nu aveți niciun nume de domeniu particularizat verificat în reclama Azure, puteți utiliza domeniul inițial Azure AD, care se termină cu *. onmicrosoft.com.
1. Asigurați-vă că numele de utilizator se află într-un domeniu care nu este federativ la Azure AD din reclama locală. Utilizatorii nu pot fi adăugați în cloud cu numele de domenii care sunt federative din local.
1. Asigurați-vă că niciun alt utilizator sau persoană de contact nu are deja numele de utilizator pe care doriți să-l atribuiți noului utilizator. Numele de utilizator trebuie să fie unice în Azure AD.
1. Consultați [rolurile AZURE AD și administratorii](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru reclama Azure.
1. Consultați [numele de domenii](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru reclama Azure.
1. Revizuiți [jurnalele de audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru a vedea mai multe informații detaliate despre un utilizator recent creat sau șters, cum ar fi cine a efectuat acțiunea și când.
1. Pentru mai multe informații despre adăugarea de utilizatori noi, consultați [utilizarea portalului Azure pentru a crea un utilizator nou în reclama Azure](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Roluri administrative AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): permisiuni de rol de administrator în Azure Active Directory
1. De asemenea, puteți [utiliza AZURE AD PowerShell pentru a crea un utilizator nou](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
