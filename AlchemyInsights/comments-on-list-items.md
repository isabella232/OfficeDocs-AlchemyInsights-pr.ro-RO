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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724166"
---
# <a name="comments-on-list-items"></a>Comentarii la elementele din listă

Utilizatorii pot să vizualizeze toate comentariile unui element de listă și să filtreze între vizualizări care afișează comentariile sau activitatea asociate unui element.

Utilizatorii trebuie să rețină următoarele înainte de a putea adăuga și șterge comentarii:

- Comentarii urmați setările de permisiune inerente în SharePoint.
- Listele clasice care nu sunt construite încă pentru a se afișa în interfețele moderne de utilizator, cum ar fi listele de activități, nu vor avea această caracteristică de comentare.
- Comentarea în listele din teams nu este disponibilă în această ediție.
- Comentariile nu sunt indexate de căutare.

Administratorii pot dezactiva această caracteristică la nivel de organizație, modificând parametrul **CommentsOnListItemsDisabled** din cmdletul **Set-SPOTenant** PowerShell.

În prezent, nu este posibil să dezactivați comentarea la site sau la nivelul listei. Sperăm să avem acele controale într-o actualizare ulterioară, probabil în primul trimestru 2021.
