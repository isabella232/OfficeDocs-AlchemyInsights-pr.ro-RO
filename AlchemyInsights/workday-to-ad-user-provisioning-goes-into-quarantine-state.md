---
title: Ziua de lucru pentru asigurarea accesului utilizatorilor AD intră în starea de carantină
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482901"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Ziua de lucru pentru asigurarea accesului utilizatorilor AD intră în starea de carantină

**Ziua de lucru pentru asigurarea accesului utilizatorilor AD intră în starea de carantină și nu se creează niciun utilizator în AD**

Lucrarea de lucru pentru asigurarea accesului utilizatorilor de zile lucrătoare a intrat în starea de carantină și jurnalele de audit afișează evenimentele nereușite de export cu eroarea mesajului de eroare **: OperationsError-SvcErr: a apărut o eroare de operațiune. Nicio referință superioară nu a fost configurată pentru serviciul director. Prin urmare, serviciul director nu poate emite referințe la obiectele din afara acestei păduri**. Această eroare apare de obicei dacă containerul Active Directory nu este setat corect sau dacă există probleme cu maparea de expresie utilizată pentru **parentDistinguishedName**.

Verificați parametrul implicit OU pentru **utilizatori noi** pentru greșeli de ortografie. Asigurați-vă că există deja un OU specificat în reclama dvs. Dacă utilizați **parentDistinguishedName** în maparea atributului, asigurați-vă că acesta se evaluează întotdeauna la un container cunoscut din domeniul de publicitate. Verificați evenimentul de export din jurnalele de audit pentru a vedea valoarea generată.

Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea accesului automat, consultați [Tutorial: Configurarea zilei de lucru pentru asigurarea accesului automat la utilizatori](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

