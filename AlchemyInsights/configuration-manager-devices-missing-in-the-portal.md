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
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817256"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="2ec30-102">Dispozitivele Manager de configurare lipsesc din portal</span><span class="sxs-lookup"><span data-stu-id="2ec30-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="2ec30-103">Pentru ca sincronizarea dispozitivelor să funcționeze, [Parametri necesare de internet](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) trebuie să fie accesibile de pe serverul local care găzduiește rolul de Punct de conexiune la serviciu.</span><span class="sxs-lookup"><span data-stu-id="2ec30-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="2ec30-104">Pentru a depana sincronizarea dispozitivelor, revizuiți **CMGatewaySyncUploadWorker.log** din punctul de conexiune la serviciu.</span><span class="sxs-lookup"><span data-stu-id="2ec30-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="2ec30-105">Aflați mai multe despre [Entitatea găzduită atașată în Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="2ec30-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
