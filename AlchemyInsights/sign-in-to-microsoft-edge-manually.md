---
title: Conectarea manuală la Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678852"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Conectarea manuală la Microsoft Edge

Dacă un utilizator nu este conectat automat în timpul unei experiențe de prima rulare, utilizatorul poate să se conecteze manual prin setările browserului sau în identitatea flyout. Pentru a gestiona conectarea, utilizați următoarele politici:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -pentru a vă asigura că un utilizator are întotdeauna un profil de lucru în Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -pentru a restricționa conectarea la un set de conturi de încredere.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -pentru a dezactiva conectarea sau pentru a obliga utilizatorii să se conecteze.

