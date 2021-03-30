---
title: Permisiuni API și procesul de consimțământ
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405438"
---
# <a name="api-permissions-and-consent-process"></a>Permisiuni API și procesul de consimțământ

Pentru ca aplicația dvs. să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să-i acorde permisiunile corecte printr-un proces de consimțământ. [Referința de permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listează permisiunile asociate cu fiecare set major de API-uri Microsoft Graph. De asemenea, oferă instrucțiuni despre cum să utilizați permisiunile.

**Set up or update service principal**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Acest articol vă arată cum să creați un nou obiect servicePrincipal.
- Crearea unui cont principal de serviciu de & pentru aplicația [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) în portal - Acest articol vă arată cum să creați o nouă aplicație și un cont principal de serviciu Azure Active Directory (Azure AD) care poate fi utilizat cu controlul accesului bazat pe roluri.
- [Directori](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) de servicii & din Azure AD - acest articol descrie înregistrarea aplicațiilor, obiectele de aplicație și informațiile principale de serviciu din Azure Active Directory: ce sunt, cum sunt utilizate și cum sunt corelate.

**Adăugați sau actualizați înregistrarea aplicațiilor și oferiți consimțământul administratorului**

- [Creați o înregistrare de aplicație](https://docs.microsoft.com/graph/api/application-post-applications) - Acest articol vă arată cum să creați un obiect de aplicație nou.
- [Actualizați o înregistrare a aplicațiilor - permisiuni API](https://docs.microsoft.com/graph/api/application-update) - acest articol vă arată cum să actualizați proprietățile unui obiect de aplicație.
- [Oferiți consimțământul administratorului](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Pentru consimțământul și consimțământul administratorului în general, este necesar ca un administrator să acordă în mod explicit consimțământul.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - container de gestionare a rolurilor pentru definiții unificate de roluri și atribuiri de roluri pentru furnizorii Microsoft 365 RBAC care acceptă mai mulți principali și domenii multiple într-o atribuire de roluri unică. Acesta este diferit de *tipul de resursă rbacApplication.* Microsoft Intune este un exemplu de astfel de furnizor RBAC. O atribuire a rolurilor în Intune poate avea o matrice de principali și o matrice de grupuri de domenii. **Acest lucru este în versiune beta, ceea ce înseamnă că este încă în dezvoltare și nu este recomandat pentru utilizare în producție.**
