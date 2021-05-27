---
title: Inventarul de software lipsește sau nu este corect
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676512"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Inventarul de software lipsește sau nu este corect

Inventarul de software din Gestiunea amenințărilor și vulnerabilităților (TVM) este o listă de software cunoscut din organizația dvs., cu liste oficiale de enumerare a platformelor comune (CPE).

Produsele software fără o CPE oficială nu au vulnerabilități publicate. Inventarul include, de asemenea, detalii precum numele furnizorului, numărul de amenințări, amenințările și numărul de dispozitive expuse.

Modificările de software de pe dispozitive se reflectă de obicei în portalurile de securitate în termen de două ore. Totuși, uneori poate dura mai mult. Momentan nu există nicio modalitate de a impune o sincronizare; este o evaluare continuă continuă.

Dacă faceți o modificare de software și modificarea nu se reflectă corect în TVM după 5 ore, urmați acești pași:

1. Verificați secțiunea de dovezi software pentru a înțelege cum a fost detectat software-ul.
1. Asigurați-vă că software-ul este acceptat. Software-ul poate fi vizibil doar la nivel de dispozitiv, chiar dacă în prezent nu este acceptat de Gestiunea amenințărilor și vulnerabilităților. Cu toate acestea, sunt disponibile doar date limitate.
1. Pentru pașii necesari raportului inaccuracy din portal, consultați [Inaccuracy raport.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Notă:** raportarea unei inadvertenări din portalul MDE este un canal uni-sens către inginerie. Dacă problema este urgentă, deschideți un tichet de asistență.

Pentru mai multe informații, consultați [Inventar software - Gestiunea amenințărilor și vulnerabilităților](/microsoft-365/security/defender-endpoint/tvm-software-inventory).