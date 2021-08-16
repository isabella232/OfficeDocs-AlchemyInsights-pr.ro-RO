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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003401"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Activarea încorporării casetelor de dialog moștenite pentru a deschide rapoarte

**Simptom**

Utilizatorii nu pot deschide rapoarte. "Ceva nu a mers bine. Consultați detaliile tehnice pentru mai multe detalii."

**Cauză**

Rapoartele nu reușesc să fie încărcate în INS cu eroarea "descriptorul de formulare este nul sau nu este definit". Rapoartele din CASETELE DE DIALOG necesită în continuare casete de dialog moștenite, prin urmare, sistemul clientului trebuie să aibă activată opțiunea *DelegacyDialogsembedding.*

**Soluție**

1. Accesați Fila **Setări >Administrare > system Setări > fila General.**

2. Setați "Activați încorporarea anumitor casete de dialog moștenite în clientul browser Interfață unificată" la **Da**.
