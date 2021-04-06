---
title: Instalarea Office și OneDrive pe Desktop virtual Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595842"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalarea Office și OneDrive pe Desktop virtual Windows

1. [Pregătirea și particularizarea unei imagini VHD coordonatoare.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Creați o mașină virtuală (VM) dacă nu a fost creată deja.

1. [Instalați Office în modul de activare a computerului partajat.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Activarea computerului partajat permite mai multor utilizatori să acceseze Office.

1. [Instalați OneDrive în modul per computer](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). În mod normal, OneDrive este instalat per utilizator, dar aici ar trebui să fie instalat pe computer.