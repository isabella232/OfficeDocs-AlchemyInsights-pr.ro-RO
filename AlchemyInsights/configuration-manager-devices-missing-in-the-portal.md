---
title: Dispozitivele Manager de configurare lipsesc din portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966121"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Dispozitivele Manager de configurare lipsesc din portal

Pentru ca sincronizarea dispozitivelor să funcționeze, [Parametri necesare de internet](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) trebuie să fie accesibile de pe serverul local care găzduiește rolul de Punct de conexiune la serviciu. Pentru a depana sincronizarea dispozitivelor, revizuiți **CMGatewaySyncUploadWorker.log** din punctul de conexiune la serviciu.

Aflați mai multe despre [Entitatea găzduită atașată în Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
