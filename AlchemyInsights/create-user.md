---
title: Crearea unui utilizator
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
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896727"
---
# <a name="create-user"></a>Crearea unui utilizator

**ANUNȚ:**

- [Perimarea suportului pentru conectare WebView de la Google începând cu 4 ianuarie 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testați dacă aplicațiile dvs. pot fi afectate [urmând instrucțiunile Google](https://go.microsoft.com/fwlink/?linkid=2157323) privind testarea compatibilității.
- Asigurați-vă că utilizați vizualizarea web sau browserul de sistem de sistem atunci când vă conectați utilizatorii cu conturi Google de larg consum. Pentru mai multe informații, [consultați Probleme la conectarea la aplicații utilizând doar browserul Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nu pot crea un utilizator nou în directorul meu Azure AD**

1. Asigurați-vă că sunteți autorizat să creați un utilizator standard nou. Doar rolul de administrator global sau de administrator de Azure Active Directory (AD) poate crea un utilizator standard nou. Dacă nu aveți unul dintre aceste roluri, solicitați unui administrator să vă adauge la unul dintre aceste roluri sau să creeze noul cont de utilizator pentru dvs.
1. Asigurați-vă că numele de utilizator se află într-un domeniu verificat în Azure AD. Dacă nu aveți niciun nume de domeniu particularizat verificat în Azure AD, puteți utiliza domeniul inițial Azure AD, care se termină cu *.onmicrosoft.com.
1. Asigurați-vă că numele de utilizator se află într-un domeniu care nu este federativ cu Azure AD din AD local. Utilizatorii nu pot fi adăugați în cloud cu nume de domeniu federative din local.
1. Asigurați-vă că niciun alt utilizator sau persoană de contact nu are deja numele de utilizator pe care doriți să-l atribuiți noului utilizator. Numele de utilizator trebuie să fie unice în Azure AD.
1. Consultați [Rolurile și administratorii Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru Azure AD.
1. Consultați numele [de domeniu](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru Azure AD.
1. Revizuiți [jurnalele de auditare](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru a vedea informații mai detaliate despre un utilizator creat recent sau șters, cum ar fi cine a efectuat acțiunea și când.
1. Pentru mai multe informații despre adăugarea de utilizatori noi, consultați [Utilizarea portalului Azure pentru a crea un utilizator nou în Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Roluri administrative Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Permisiuni de rol de administrator în Azure Active Directory
1. De asemenea, [puteți utiliza Azure AD PowerShell pentru a crea un utilizator nou.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
