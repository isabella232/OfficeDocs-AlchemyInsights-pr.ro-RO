---
title: Offboard non-dispozitivele Windows de la Microsoft Defender-protecție avansată împotriva amenințărilor (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748480"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-dispozitivele Windows de la Microsoft Defender-protecție avansată împotriva amenințărilor (ATP)

Iată cum se procedează:

1. Urmați documentația de la terți pentru deconectarea soluției de la terți de la Microsoft Defender ATP.
2. De la entitatea găzduită Azure Active Directory, eliminați permisiunile pentru soluția de la terți:

    1. Conectați-vă la [portalul Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Selectare **totală servicii**  >  **Azure Active Directory**  >  **Enterprise Applications**.
    1. Selectați aplicația pe care doriți să o offboard.
    1. Selectați **Ștergere**.

Pentru a afla mai multe, consultați [offboard dispozitivelor non-Windows](https://go.microsoft.com/fwlink/?linkid=2143630).
