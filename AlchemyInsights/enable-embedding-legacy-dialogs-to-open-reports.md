---
title: Activarea încorporării casetelor de dialog moștenite pentru a deschide rapoarte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814276"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Activarea încorporării casetelor de dialog moștenite pentru a deschide rapoarte

**Simptom**

Utilizatorii nu pot deschide rapoarte. "Ceva nu a mers bine. Consultați detaliile tehnice pentru mai multe detalii."

**Cauză**

Rapoartele nu reușesc să fie încărcate în INS cu eroarea "descriptorul de formulare este nul sau nu este definit". Rapoartele din CASETELE DE DIALOG necesită în continuare casete de dialog moștenite, prin urmare, sistemul clientului trebuie să aibă activată opțiunea *DelegacyDialogsembedding.*

**Soluție**

1. Accesați Setări **>Administrare > System Settings (Setări > fila General).**

2. Setați "Activați încorporarea anumitor casete de dialog moștenite în clientul browser Interfață unificată" la **Da**.
