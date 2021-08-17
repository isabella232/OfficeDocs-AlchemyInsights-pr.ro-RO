---
title: Conectați-vă la Microsoft Edge automat
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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050706"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Conectați-vă la Microsoft Edge automat

Microsoft Edge utilizează contul implicit OS pentru a se conecta automat la un utilizator în funcție de modul în care este configurat dispozitivul utilizatorului. 

Scenariile pentru fiecare tip de configurare a dispozitivului și procesul său dependent de conectare al utilizatorului sunt descrise mai jos:

- **Dispozitivul este hibrid/AAD-J:** această opțiune este disponibilă pe versiunile de Windows 10, de nivel Windows și de server corespunzătoare. Utilizatorii sunt conectați automat cu conturile Azure Active Directory (AD).
- **Dispozitivul este unit cu domeniul:** această opțiune este disponibilă pe versiunile Windows 10, versiunile de Windows și versiunile corespunzătoare de server. În mod implicit, utilizatorii cu conturi de domeniu nu sunt conectați automat; pentru a activa conectarea automată pentru ei, utilizați **politica ConfigureOnPremisesAccountAutoSignIn.** Pentru a activa conectarea automată pentru utilizatorii cu conturi Azure AD, luați în considerare asocierea hibridă la dispozitivele lor.
- Contul implicit al unui sistem de operare este un cont **Microsoft:** această opțiune este disponibilă pe Windows 10 RS3 (versiunea 1709, versiunea 10.0.16299) și versiunile mai recente. Scenariul este puțin probabil să apară pe dispozitivele de întreprindere. Cu toate acestea, în cazul în care contul implicit al sistemul de operare este un cont Microsoft, Microsoft Edge va conecta automat utilizatorul cu contul Microsoft.
 
 
