---
title: Instrucțiuni generale despre performanța migrării
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932490"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="17d72-102">Instrucțiuni generale despre performanța migrării</span><span class="sxs-lookup"><span data-stu-id="17d72-102">General migration performance guidance</span></span>

<span data-ttu-id="17d72-103">**Important**: Mulți clienți SharePoint Online și OneDrive rulează aplicații critice pentru firmă împotriva serviciului care rulează în fundal.</span><span class="sxs-lookup"><span data-stu-id="17d72-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="17d72-104">Printre acestea se numără migrarea conținutului, Prevenirea Pierderii Datelor (DLP) și soluțiile de backup.</span><span class="sxs-lookup"><span data-stu-id="17d72-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="17d72-105">În aceste timpuri fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de accesibile și fiabile pentru utilizatorii dvs. care depind de serviciu mai mult ca oricând în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="17d72-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="17d72-106">Pentru a susține acest obiectiv, am implementat limite mai stricte pentru aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de lucru din zilele lucrătoare.</span><span class="sxs-lookup"><span data-stu-id="17d72-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="17d72-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un randament foarte limitat în aceste ore.</span><span class="sxs-lookup"><span data-stu-id="17d72-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="17d72-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="17d72-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="17d72-109">**Instrucțiuni pentru performanța migrării**</span><span class="sxs-lookup"><span data-stu-id="17d72-109">**Migration performance guidance**</span></span>

<span data-ttu-id="17d72-110">Performanța de migrare poate fi influențată de infrastructura de rețea, de dimensiunea fișierului, timpul de migrare și de limitare.</span><span class="sxs-lookup"><span data-stu-id="17d72-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="17d72-111">Înțelegerea acestora vă va ajuta să planificați și să maximizați eficiența migrării dvs.</span><span class="sxs-lookup"><span data-stu-id="17d72-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="17d72-112">Instrucțiuni generale despre performanța migrării</span><span class="sxs-lookup"><span data-stu-id="17d72-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
