---
title: Trimiteți notificări personalizate cu Intune
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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086176"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Cum să trimiteți notificări personalizate utilizatorilor dispozitivelor iOS și Android gestionate

Notificările particularizate pentru Intune sunt procesate de Portal firmă app pe dispozitivul unui utilizator. Aplicația creează apoi notificarea push pe acel dispozitiv.

În cele ce urmează sunt cerințe preliminare pentru dispozitiv, pentru a permite confirmarea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea push:

- Dispozitivul trebuie să aibă instalată Portal firmă instalată.  

- Dispozitivul trebuie să permită aplicației Portal firmă să trimită notificări push. Atunci când aplicația este instalată sau actualizată, îi va solicita utilizatorului să permită notificări.

- Dispozitivele Android trebuie să aibă instalate serviciile Google Play.

- Dispozitivul trebuie înregistrat cu Intune.

Pentru mai multe informații, inclusiv despre cum să trimiteți un mesaj, consultați [documentația despre caracteristici.](https://docs.microsoft.com/intune/custom-notifications)
