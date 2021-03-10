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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695157"
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
