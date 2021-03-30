---
title: Configurarea setărilor de confidențialitate în Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405735"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="070c8-102">Configurarea setărilor de confidențialitate în Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="070c8-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="070c8-103">În mod implicit, dacă Microsoft Edge este implementat pe platformele non-Windows, datele de diagnosticare și informațiile despre site nu sunt trimise la Microsoft.</span><span class="sxs-lookup"><span data-stu-id="070c8-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="070c8-104">Cu toate acestea, dacă Microsoft Edge este implementat în Windows 10, datele de diagnosticare și informațiile despre site sunt trimise în conformitate cu setările de [date Diagnosticare Windows ale utilizatorilor.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="070c8-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="070c8-105">Pentru a configura modul în care Microsoft Edge gestionează colectarea datelor pentru organizația dvs., utilizați următoarele politici de grup:</span><span class="sxs-lookup"><span data-stu-id="070c8-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="070c8-106">[MetricsReportingEnabled activează](https://go.microsoft.com/fwlink/?linkid=2132470) raportarea utilizării și a datelor legate de cădere.</span><span class="sxs-lookup"><span data-stu-id="070c8-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="070c8-107">[SendSiteInfoToImproveServices trimite informațiile](https://go.microsoft.com/fwlink/?linkid=2132470) de site utilizate pentru a îmbunătăți serviciile Microsoft.</span><span class="sxs-lookup"><span data-stu-id="070c8-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="070c8-108">Pentru mai multe informații, consultați [Configurarea setărilor de politică.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="070c8-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
