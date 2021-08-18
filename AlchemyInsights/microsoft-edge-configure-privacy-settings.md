---
title: Microsoft Edge configurați setările de confidențialitate
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114184"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurați setările de confidențialitate

În mod implicit, dacă Microsoft Edge implementate pe platforme non-Windows, datele de diagnosticare și informațiile despre site nu sunt trimise la Microsoft. Cu toate acestea, Microsoft Edge sunt implementate pe Windows 10, datele de diagnosticare și informațiile despre site sunt trimise în conformitate cu setările de date [de Windows Diagnostic.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Pentru a configura Microsoft Edge de colectare a datelor pentru organizația dvs., utilizați următoarele politici de grup:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Această politică permite raportarea utilizării și a datelor legate de cădere.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Această politică trimite informații despre site care sunt utilizate pentru a servicii Microsoft.

Pentru mai multe informații, consultați [Configurarea setărilor de politică.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)