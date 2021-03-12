---
title: Remedierea regulilor de transport
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750577"
---
# <a name="fix-transport-rules"></a>Remedierea regulilor de transport

O regulă de flux de corespondență particularizată A afectat acest mesaj. Pentru a revizui regula exactă, procedați astfel:

1. În rezultatele remiterii, sub **informații suplimentare**, notați **GUID** -ul sau **numele politicii**.
2. Lansați componenta de administrare Exchange. Pentru mai multe informații, consultați [Deschideți componenta de administrare Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Rularea acestei comenzi (utilizând GUID-ul de la prezentarea dvs.):  **Get-TransportRule-Identity "GUID" | FL * Descriere***
4. Revizuiți Descrierea pentru a vedea condițiile configurate care au afectat mesajul.

Pentru a afla mai multe, consultați [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
