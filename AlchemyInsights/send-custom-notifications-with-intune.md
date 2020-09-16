---
title: Trimiterea de notificări particularizate cu Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720658"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cum să trimiteți notificări particularizate utilizatorilor de dispozitive iOS și Android gestionate

Notificările particularizate pentru Intune sunt prelucrate de aplicația portal a firmei pe dispozitivul unui utilizator. Aplicația creează apoi notificarea Push pe acel dispozitiv.

Următoarele sunt cerințe preliminare pentru dispozitive pentru a accepta primirea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea Push:

- Dispozitivul trebuie să aibă instalată aplicația portal firmă.  

- Dispozitivul trebuie să permită aplicației portal a firmei să trimită notificări Push. Atunci când aplicația este instalată sau actualizată, aceasta va solicita utilizatorului să autorizeze notificările.

- Dispozitivele Android trebuie să aibă instalat Google Play Services.

- Dispozitivul trebuie să fie înscris cu Intune.

Pentru mai multe informații, inclusiv cum să trimiteți un mesaj, consultați [documentația caracteristicii](https://docs.microsoft.com/intune/custom-notifications).
