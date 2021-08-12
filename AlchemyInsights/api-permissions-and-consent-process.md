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
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932073"
---
# <a name="api-permissions-and-consent-process"></a>Permisiuni API și procesul de consimțământ

Pentru ca aplicația dvs. să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să-i acorde permisiunile corecte printr-un proces de consimțământ. [Referința Graph permisiuni microsoft](https://docs.microsoft.com/graph/permissions-reference) listează permisiunile asociate cu fiecare set major de API-uri Graph Microsoft. De asemenea, oferă instrucțiuni despre cum să utilizați permisiunile.

**Set up or update service principal**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - Acest articol vă arată cum să creați un nou obiect servicePrincipal.
- Crearea unui cont principal de serviciu & pentru aplicația [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) în portal - Acest articol vă arată cum să creați o nouă aplicație și un cont principal de serviciu Azure Active Directory (Azure AD) care poate fi utilizat cu controlul accesului bazat pe rol.
- [Directori](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) de servicii & din Azure AD - acest articol descrie înregistrarea aplicațiilor, obiectele de aplicație și furnizorii principali de serviciu din Azure Active Directory: ce sunt, cum sunt utilizate și cum sunt corelate.

**Adăugați sau actualizați înregistrarea aplicațiilor și oferiți consimțământul administratorului**

- [Creați o înregistrare de aplicație](https://docs.microsoft.com/graph/api/application-post-applications) - Acest articol vă arată cum să creați un obiect de aplicație nou.
- [Actualizați o înregistrare a aplicațiilor - permisiuni API](https://docs.microsoft.com/graph/api/application-update) - acest articol vă arată cum să actualizați proprietățile unui obiect de aplicație.
- [Oferiți consimțământul administratorului](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Pentru consimțământul și consimțământul administratorului în general, este necesar ca un administrator să acordă în mod explicit consimțământul.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - container de gestionare a rolurilor pentru definiții unificate de roluri și atribuiri de roluri pentru furnizorii Microsoft 365 RBAC care acceptă mai mulți principali și domenii multiple într-o atribuire de roluri unică. Acesta este diferit de *tipul de resursă rbacApplication.* Microsoft Intune un exemplu de astfel de furnizor RBAC. O atribuire a rolurilor în Intune poate avea o matrice de principali și o matrice de grupuri de domenii. **Acest lucru este în versiune beta, ceea ce înseamnă că este încă în dezvoltare și nu este recomandat pentru utilizare în producție.**
