---
title: Comentarii la elementele din listă
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982560"
---
# <a name="comments-on-list-items"></a>Comentarii la elementele din listă

Utilizatorii vor putea în curând să adauge și să șteargă comentarii în elementele din listă. Utilizatorii pot să vizualizeze toate comentariile unui element de listă și să filtreze între vizualizări care afișează comentariile sau activitatea asociate unui element.

**Temporizare** :

**Lansare specifică** : roll progresiv în Mid-octombrie și se așteaptă să se finalizeze până la mijlocul lunii noiembrie

**Ediție standard** : roll treptat la mijlocul lunii noiembrie și se așteaptă să se finalizeze până la începutul lunii decembrie

**Implementare** : lansare specifică pentru întreaga organizație

Utilizatorii trebuie să rețină următoarele înainte de a putea adăuga și șterge comentarii:

- Comentarii urmați setările de permisiune inerente în SharePoint.
- Listele clasice care nu sunt construite încă pentru a se afișa în interfețele moderne de utilizator, cum ar fi listele de activități, nu vor avea această caracteristică de comentare.
- Comentarea în listele din teams nu este disponibilă în această ediție.
- Comentariile nu sunt indexate de căutare.

Administratorii pot dezactiva această caracteristică la nivel de organizație, modificând parametrul **CommentsOnListItemsDisabled** din cmdletul **Set-SPOTenant** PowerShell.

În prezent, nu este posibil să dezactivați comentarea la site sau la nivelul listei. Sperăm să avem acele controale într-o actualizare ulterioară, probabil în primul trimestru 2021.
