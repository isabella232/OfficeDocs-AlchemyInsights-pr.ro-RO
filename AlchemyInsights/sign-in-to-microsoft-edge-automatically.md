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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398741"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Conectarea automată la Microsoft Edge

Microsoft Edge utilizează contul implicit al unui sistem de operare pentru a se conecta automat la un utilizator, în funcție de modul în care este configurat dispozitivul utilizatorului. 

Scenariile pentru fiecare tip de configurare a dispozitivului și procesul său dependent de conectare al utilizatorului sunt descrise mai jos:

- **Dispozitivul este hibrid/AAD-J:** această opțiune este disponibilă în Windows 10, versiunile de nivel inferior windows și versiunile de server corespunzătoare. Utilizatorii sunt conectați automat cu conturile lor Azure Active Directory (AD).
- **Dispozitivul este unit cu domeniul:** această opțiune este disponibilă în Windows 10, în windows de nivel inferior și în versiunile de server corespunzătoare. În mod implicit, utilizatorii cu conturi de domeniu nu sunt conectați automat; pentru a activa conectarea automată pentru ei, utilizați **politica ConfigureOnPremisesAccountAutoSignIn.** Pentru a activa conectarea automată pentru utilizatorii cu conturi Azure AD, luați în considerare asocierea hibridă la dispozitivele lor.
- Contul implicit al sistemului de operare este un cont **Microsoft:** această opțiune este disponibilă în Windows 10 RS3 (versiunea 1709, versiunea 10.0.16299) și versiunile mai recente. Scenariul este puțin probabil să apară pe dispozitivele de întreprindere. Cu toate acestea, în cazul în care contul implicit al unui sistem de operare este un cont Microsoft, Microsoft Edge va conecta automat utilizatorul cu contul Microsoft.
 
 
