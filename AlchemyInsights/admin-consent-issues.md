---
title: Probleme cu consimțământul administratorului
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901509"
---
# <a name="admin-consent-issues"></a>Probleme cu consimțământul administratorului

1. Activați [fluxul de lucru pentru consimțământul administratorului](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) pentru a permite utilizatorilor să solicite aprobarea de administrator direct din ecranul de consimțământ.

1. Dacă dumneavoastră sau utilizatorii aplicației Vedeți erori neașteptate în timpul procesului de consimțământ, consultați acest articol pentru pașii de depanare: [Eroare neașteptată atunci când efectuați consimțământul pentru o aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Aflați mai multe despre [consimțământul administratorului pe platforma de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), modul în care funcționează [solicitarea de aprobare](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) și cum să [evaluați o solicitare pentru consimțământul administratorului la nivel de entitate găzduită](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplicațiile care se integrează cu platforma de identitate Microsoft urmăresc un model de autorizare care le oferă utilizatorilor și administratorilor controlul asupra modului în care pot fi accesate datele. Implementarea modelului de autorizare a fost actualizată pe punctul final al platformei de identitate Microsoft și schimbă modul în care o aplicație trebuie să interacționeze cu platforma de identitate Microsoft. Vedeți [permisiunile și consimțământul în punctul final al platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) pentru o prezentare generală a acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.