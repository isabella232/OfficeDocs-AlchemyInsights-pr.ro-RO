---
title: Conectarea automată la Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678813"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Conectarea automată la Microsoft Edge

Microsoft Edge utilizează contul implicit al sistemului de operare pentru a se conecta automat la un utilizator în funcție de modul în care este configurat dispozitivul utilizatorului. 

Scenariile pentru fiecare tip de configurație a dispozitivului și procesul de conectare la utilizatorul său dependent sunt descrise mai jos:

1. **Dispozitivul este hibrid/AAD-J**: această opțiune este disponibilă în Windows 10, Windows level și versiunile de server corespunzătoare. Utilizatorii sunt conectați automat cu conturile lor Azure Active Directory (AD).
2. **Dispozitivul este asociat domeniului**: această opțiune este disponibilă în Windows 10, Windows level și versiunile de server corespondente. În mod implicit, utilizatorii cu conturi de domeniu nu sunt conectați automat; pentru a activa conectarea automată pentru ele, utilizați Politica **ConfigureOnPremisesAccountAutoSignIn** . Pentru a activa conectarea automată pentru utilizatori cu conturi de publicitate Azure, luați în considerare conectarea hibridă a dispozitivelor.
3. **Contul implicit al sistemului de operare este un cont Microsoft**: această opțiune este disponibilă în Windows 10 RS3 (versiunea 1709, compilarea 10.0.16299) și versiunile ulterioare. Scenariul este puțin probabil să apară pe dispozitivele Enterprise. Cu toate acestea, dacă contul implicit al sistemului de operare este un cont Microsoft, atunci Microsoft Edge se va conecta automat la utilizator cu contul Microsoft.
 
 
