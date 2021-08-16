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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034766"
---
# <a name="fix-transport-rules"></a>Remedierea regulilor de transport

O regulă de flux de corespondență particularizată a afectat acest mesaj. Pentru a revizui regula exactă, acțiunile următoare:

1. În rezultatele remiterii, sub **Informații suplimentare,** notați **GUID-ul** sau **Numele politicii.**
2. Lansați Exchange de administrare. Pentru mai multe informații, [consultați Deschiderea Exchange de administrare .](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Rulați această comandă (utilizând GUID-ul din remitere):  **Get-TransportRule -identity "GUID" | fl * Descriere***
4. Revizuiți descrierea pentru a vedea condițiile configurate care au afectat mesajul.

Pentru a afla mai multe, [consultați Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
