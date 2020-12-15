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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="df26c-102">Microsoft Edge configurează setările de confidențialitate</span><span class="sxs-lookup"><span data-stu-id="df26c-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="df26c-103">În mod implicit, dacă Microsoft Edge este implementat pe platforme non-Windows, datele de diagnosticare și informațiile despre site nu sunt trimise la Microsoft.</span><span class="sxs-lookup"><span data-stu-id="df26c-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="df26c-104">Cu toate acestea, dacă Microsoft Edge este implementat în Windows 10, datele de diagnosticare și informațiile de site sunt trimise conform [setărilor de date de diagnosticare Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)ale utilizatorilor.</span><span class="sxs-lookup"><span data-stu-id="df26c-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="df26c-105">Pentru a configura modul în care Microsoft Edge manipulează colectarea de date pentru organizația dvs., utilizați următoarele politici de grup:</span><span class="sxs-lookup"><span data-stu-id="df26c-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="df26c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): această politică permite raportarea utilizării și a datelor legate de căderi.</span><span class="sxs-lookup"><span data-stu-id="df26c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="df26c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): această politică trimite informații despre site care se utilizează pentru a îmbunătăți serviciile Microsoft.</span><span class="sxs-lookup"><span data-stu-id="df26c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="df26c-108">Pentru a afla mai multe, consultați [Configurarea setărilor de politică](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="df26c-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>