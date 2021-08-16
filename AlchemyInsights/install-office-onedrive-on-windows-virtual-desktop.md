---
title: Instalarea Office și OneDrive pe Windows Desktop virtual
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
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028628"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalarea Office și OneDrive pe Windows Desktop virtual

1. [Pregătirea și particularizarea unei imagini VHD coordonatoare.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Creați o mașină virtuală (VM) dacă nu a fost creată deja.

1. [Instalați Office în modul de activare a computerului partajat.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Activarea computerului partajat permite mai multor utilizatori să Office.

1. [Instalați OneDrive în modul per computer](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). În mod normal, OneDrive sunt instalate per utilizator, dar aici ar trebui să fie instalate pe fiecare computer.