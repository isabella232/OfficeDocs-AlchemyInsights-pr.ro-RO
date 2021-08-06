---
title: Workday to AD User Provisioning goes in quarantine state
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036504"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday to AD User Provisioning goes in quarantine state

**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**

Activitatea De zi de lucru la Asigurare acces pentru utilizatorii AD a dispărut în starea de carantină, iar jurnalele de auditare arată evenimentele de eroare de export cu mesajul de eroare **Eroare: OperationsError-SvcErr: Eroare de operațiune. Nu a fost configurată nicio referință superioară pentru serviciul director. Serviciul director nu poate, prin urmare, să emită recomandări către obiectele din afara acestei păduri**. Această eroare apare de obicei dacă Active Directory Container OU nu este setat corect sau dacă există probleme cu Maparea expresiilor utilizată pentru **parentDistinguishedName**.

Verificați parametrul OU implicit pentru **utilizatori noi** pentru tastare. Asigurați-vă că OU-ul specificat există deja în AD. Dacă utilizați **parentDistinguishedName** în maparea atributului, asigurați-vă că acesta se evaluează întotdeauna la un container cunoscut din domeniul AD. Verificați evenimentul Export din jurnalele de auditare pentru a vedea valoarea generată.

Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea automată a accesului, consultați Tutorial: Configurarea zilei de lucru pentru asigurarea automată [a accesului utilizatorilor.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

