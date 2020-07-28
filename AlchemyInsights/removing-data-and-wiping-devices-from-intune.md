---
title: Eliminarea datelor și ștergerea dispozitivelor din Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440469"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Eliminarea datelor și ștergerea dispozitivelor din Intune

Acțiunile de la distanță Pentru retragerea dispozitivului și ștergerea dispozitivului pot fi utilizate pentru a elimina datele companiei gestionate de Intune sau pentru a efectua o resetare din fabrică și pentru a readuce dispozitivul la setările sale implicite.

1. Conectați-vă la Microsoft 365 **Devices**Device Management și accesați  >  **Devices All Devices**.
2. Selectați dispozitivul pe care doriți să-l ștergeți.
3. Selectați tipul de ștergere la distanță pe care doriți să îl faceți. Retragere șterge numai informațiile organizaționale, în timp ce șervețelele complete restabilesc dispozitivul la setările sale din fabrică.
4. Selectați **Da** pentru confirmare. Până la terminarea ștergerii, starea acțiunii Dispozitiv se afișează ca Retragere în așteptare.</br>
    După terminarea acțiunii, nu veți mai vedea dispozitivul mobil în lista de dispozitive gestionate.

**Notă** Datele companiei nu pot fi eliminate de pe dispozitivele ASOCIATE în Azure AD.

Pentru detalii complete despre efectul acțiunilor Retragere și ștergere, inclusiv ce este reținut și ce este șters, consultați [Eliminarea dispozitivelor utilizând ștergerea, retragerea sau anularea manuală a dispozitivului](https://docs.microsoft.com/intune/devices-wipe).

Pentru a șterge toate datele de pe un dispozitiv macOS, consultați [Ștergerea tuturor datelor de pe un dispozitiv macOS](https://docs.microsoft.com/intune/device-erase).