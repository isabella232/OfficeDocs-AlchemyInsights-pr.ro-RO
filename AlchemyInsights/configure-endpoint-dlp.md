---
title: Configurați Microsoft Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657941"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f6d64-102">Configurați Microsoft Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="f6d64-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f6d64-103">Microsoft Endpoint DLP vă permite să extindeți capacitatea de monitorizare și protecție DLP la informații confidențiale pe dispozitivele Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f6d64-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f6d64-104">După înscrierea dispozitivelor în Gestionarea dispozitivelor, puteți crea politici DLP pentru a impune acțiuni de protecție pentru elemente.</span><span class="sxs-lookup"><span data-stu-id="f6d64-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f6d64-105">Exploratorul de activități poate fi utilizat pentru a monitoriza activitatea pentru elementele confidențiale.</span><span class="sxs-lookup"><span data-stu-id="f6d64-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f6d64-106">Pentru mai multe informații, consultați [Înscrierea dispozitivelor în Gestionarea dispozitivelor](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="f6d64-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f6d64-107">Pentru a începe lucrul cu Microsoft Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="f6d64-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f6d64-108">Asigurați-vă că aveți licențierea corespunzătoare pentru SKU/abonamente.</span><span class="sxs-lookup"><span data-stu-id="f6d64-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f6d64-109">Pentru mai multe informații, consultați [Licențierea pentru SKU/abonamente](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f6d64-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f6d64-110">Verificați permisiunile necesare pentru a activa gestionarea dispozitivelor, pentru accesa pagina de înscriere sau a activa/dezactiva monitorizarea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="f6d64-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f6d64-111">Pentru mai multe informații, consultați [Permisiuni](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="f6d64-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f6d64-112">Înscrieți dispozitive în Gestionarea dispozitivelor, urmând procedura pentru înscrierea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="f6d64-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f6d64-113">Pentru mai multe informații, consultați [Înscrierea dispozitivelor](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="f6d64-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f6d64-114">Creați politici DLP pentru a vă proteja elementele confidențiale.</span><span class="sxs-lookup"><span data-stu-id="f6d64-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f6d64-115">Pentru informații, consultați [Scenarii de politică Microsoft Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f6d64-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="f6d64-116">Pentru mai multe informații despre Microsoft Endpoint DLP, consultați [Aflați despre măsurile de prevenire a pierderii datelor Microsoft 365 Endpoint (previzualizare)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="f6d64-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f6d64-117">**Pași importanți de colectare a datelor, dacă este necesară asistența:**</span><span class="sxs-lookup"><span data-stu-id="f6d64-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f6d64-118">Descărcați [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="f6d64-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="f6d64-119">Rulați instrumentul ca administrator din fereastra cmd:</span><span class="sxs-lookup"><span data-stu-id="f6d64-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="f6d64-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="f6d64-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="f6d64-121">Când vi se solicită cu Introduceți numărul de minute de colectare a **trasării:**, introduceți numărul de minute necesare pentru a rula scenariul.</span><span class="sxs-lookup"><span data-stu-id="f6d64-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="f6d64-122">Rulați scenariul.</span><span class="sxs-lookup"><span data-stu-id="f6d64-122">Run the scenario.</span></span>

<span data-ttu-id="f6d64-123">Colectați rezultatul fișierului zip pentru a-l oferi agentului de asistență.</span><span class="sxs-lookup"><span data-stu-id="f6d64-123">Collect the Zip file output to give to the Support agent.</span></span>
