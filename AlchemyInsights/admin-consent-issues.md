---
title: Probleme legate de consimțământul administratorului
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952585"
---
# <a name="admin-consent-issues"></a>Probleme legate de consimțământul administratorului

1. Activați fluxul [de lucru pentru consimțământul administratorului](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) pentru a le permite utilizatorilor să solicite aprobarea administratorului direct din ecranul de consimțământ.

1. Dacă dvs. sau utilizatorii aplicației dvs. vedeți erori neașteptate în timpul procesului de consimțământ, consultați acest articol pentru pașii de depanare: Eroare neașteptată la efectuarea consimțământului [pentru o aplicație.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Aflați mai multe [despre Consimțământul administratorului pentru Serviciu de identitate Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)modul în care funcționează solicitarea de consimțământ și cum să evaluați o solicitare pentru consimțământul [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [administratorului la nivel de entitate găzduită.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Aplicațiile care se integrează cu Serviciu de identitate Microsoft urmează un model de autorizare care le oferă utilizatorilor și administratorilor control asupra modului în care pot fi accesate datele. Implementarea modelului de autorizare a fost actualizată în punctul final Serviciu de identitate Microsoft autorizare și modifică modul în care trebuie să interacționeze o aplicație cu Serviciu de identitate Microsoft. Consultați [Permisiuni și consimțământ în Serviciu de identitate Microsoft final pentru](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) o prezentare generală a acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.