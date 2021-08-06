---
title: Eliminarea datelor și ștergerea dispozitivelor din Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922259"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Eliminarea datelor și ștergerea dispozitivelor din Intune

Acțiunile la distanță de retragere și ștergere a dispozitivului pot fi utilizate pentru a elimina datele firmei gestionate de Intune sau pentru a efectua o reinițializare la setările din fabrică și a restabili setările implicite pe dispozitiv.

1. Conectați-vă la Microsoft 365 Management și accesați **Dispozitive** > **Toate dispozitivele**.
2. Selectați dispozitivul pe care doriți să îl ștergeți.
3. Selectați tipul de ștergere de la distanță pe care doriți să o efectuați. Retragerea șterge numai informațiile organizației, în timp ce ștergerile complete restaurează dispozitivul la setările din fabrică.
4. Selectați **Da** pentru a confirma. Până când se termină ștergerea, starea acțiunii pentru dispozitiv se afișează ca *În aşteptarea retragerii*.
    După ce se încheie acțiunea, nu veți mai vedea dispozitivul mobil în lista de dispozitive gestionate.

> [!NOTE]
> Datele firmei nu pot fi eliminate de pe dispozitivele ASOCIATE la Azure AD. 

Pentru detalii complete cu privire la efectul acțiunilor de retragere și ștergere, inclusiv elementele păstrate și cele șterse, consultați documentația următoare:

- [Eliminarea dispozitivelor utilizând ștergerea, retragerea sau anularea manuală a înscrierii dispozitivului](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Cum să ștergeți doar datele corporației din aplicațiile gestionate de Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Ștergeți toate datele de pe un dispozitiv macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).