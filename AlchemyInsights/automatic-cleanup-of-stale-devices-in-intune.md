---
title: Curățarea automată a dispozitivelor învechite în Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555228"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Curățarea automată a dispozitivelor învechite în Intune

Intune permite administratorului să configureze un interval de timp între 90 și 270 de zile, după care dispozitivele învechite sunt eliminate din serviciu. Această setare este la nivel de organizare și o dată activat intră în vigoare imediat. Toate dispozitivele care nu au fost verificate în serverul Intune pentru o perioadă care depășește setarea sunt șterse definitiv.

**Notă** Numai obiectele de dispozitiv MDM sunt eligibile pentru această acțiune de curățare. Sunt excluse numai obiectele dispozitivului EAS.

Pentru informații suplimentare despre momentul în care un dispozitiv devine eligibil pentru ștergere pe baza setării de curățare a dispozitivului și a "stării" acestuia:

Setare: **Ștergerea dispozitivelor după ultima dată de check-in: Da (o anumită valoare (N) în zilele specificate)**

- Pe baza valorii (N) configurate în setare, serviciul Intune șterge dispozitivul în zilele specificate după ultima verificare reușită.

Setare: **Ștergerea dispozitivelor după ultima dată de check-in: Nu**

- La 180 de zile de la expirarea certificatului dispozitivului și nu este reînnoit, dispozitivul este șters.

**Notă** În ambele cazuri, dispozitivul trebuie înregistrat cu succes în Intune. Înregistrarea are loc în timpul primei verificări a dispozitivului cu serviciul Intune.

Dacă un dispozitiv se înscrie cu succes la Intune, dar nu devine înregistrat Intune, dispozitivul este șters la 270 de zile de la înscriere. (90 de zile pentru a marca dispozitivul ca revocat, apoi alte 180 de zile pentru a șterge înregistrarea.)

Nu există niciun mecanism în prezent în consola Intune pentru a stabili data de expirare a certificării dispozitivului pentru un anumit dispozitiv.