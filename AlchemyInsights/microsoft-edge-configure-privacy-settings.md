---
title: Microsoft Edge configurează setările de confidențialitate
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
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678857"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurează setările de confidențialitate

În mod implicit, dacă Microsoft Edge este implementat pe platforme non-Windows, datele de diagnosticare și informațiile despre site nu sunt trimise la Microsoft. Cu toate acestea, dacă Microsoft Edge este implementat în Windows 10, datele de diagnosticare și informațiile de site sunt trimise conform [setărilor de date de diagnosticare Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)ale utilizatorilor.

Pentru a configura modul în care Microsoft Edge manipulează colectarea de date pentru organizația dvs., utilizați următoarele politici de grup:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): această politică permite raportarea utilizării și a datelor legate de căderi.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): această politică trimite informații despre site care se utilizează pentru a îmbunătăți serviciile Microsoft.

Pentru a afla mai multe, consultați [Configurarea setărilor de politică](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).