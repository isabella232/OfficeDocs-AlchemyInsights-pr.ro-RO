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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402447"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3f60b-102">Configurați Microsoft Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="3f60b-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3f60b-103">Microsoft Endpoint DLP vă permite să extindeți capacitatea de monitorizare și protecție DLP la informații confidențiale pe dispozitivele Windows 10.</span><span class="sxs-lookup"><span data-stu-id="3f60b-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3f60b-104">După înscrierea dispozitivelor în Gestionarea dispozitivelor, puteți crea politici DLP pentru a impune acțiuni de protecție pentru elemente.</span><span class="sxs-lookup"><span data-stu-id="3f60b-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3f60b-105">Exploratorul de activități poate fi utilizat pentru a monitoriza activitatea pentru elementele confidențiale.</span><span class="sxs-lookup"><span data-stu-id="3f60b-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3f60b-106">Pentru mai multe informații, consultați [Înscrierea dispozitivelor în Gestionarea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="3f60b-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3f60b-107">Pentru a începe lucrul cu Microsoft Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="3f60b-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3f60b-108">Asigurați-vă că aveți licențierea corespunzătoare pentru SKU/abonamente.</span><span class="sxs-lookup"><span data-stu-id="3f60b-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3f60b-109">Pentru mai multe informații, consultați [Licențierea pentru SKU/abonamente](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="3f60b-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3f60b-110">Verificați permisiunile necesare pentru a activa gestionarea dispozitivelor, pentru accesa pagina de înscriere sau a activa/dezactiva monitorizarea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="3f60b-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="3f60b-111">Pentru mai multe informații, consultați [Permisiuni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="3f60b-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3f60b-112">Înscrieți dispozitive în Gestionarea dispozitivelor, urmând procedura pentru înscrierea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="3f60b-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3f60b-113">Dacă lipsește opțiunea Înscrierea dispozitivelor (previzualizare) sub Conformitate M365  **Setări**, confirmați că aveți licența și permisiunile corespunzătoare la care s-a făcut referire mai sus.</span><span class="sxs-lookup"><span data-stu-id="3f60b-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="3f60b-114">Pentru mai multe informații, consultați [Înscrierea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="3f60b-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3f60b-115">Creați politici DLP pentru a vă proteja elementele confidențiale.</span><span class="sxs-lookup"><span data-stu-id="3f60b-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3f60b-116">Pentru informații, consultați [Scenarii de politică Microsoft Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="3f60b-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="3f60b-117">Pentru mai multe informații despre Microsoft Endpoint DLP, consultați [Aflați despre măsurile de prevenire a pierderii datelor Microsoft 365 Endpoint (previzualizare)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="3f60b-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="3f60b-118">**Pași importanți de colectare a datelor, dacă este necesară asistența:**</span><span class="sxs-lookup"><span data-stu-id="3f60b-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="3f60b-119">Descărcați MDATP Client Analyzer Preview de la [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="3f60b-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="3f60b-120">Rulați instrumentul ca administrator din fereastra cmd:</span><span class="sxs-lookup"><span data-stu-id="3f60b-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="3f60b-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="3f60b-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="3f60b-122">Când vi se solicită „Introduceți numărul de minute pentru a colecta trasarea: ”, introduceți numărul de minute necesare pentru a rula scenariul</span><span class="sxs-lookup"><span data-stu-id="3f60b-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="3f60b-123">Rulați scenariul</span><span class="sxs-lookup"><span data-stu-id="3f60b-123">Run the scenario</span></span>

<span data-ttu-id="3f60b-124">Colectați rezultatul fișierului zip de trimis agentului de asistență.</span><span class="sxs-lookup"><span data-stu-id="3f60b-124">Collect the Zip file output to be given to the Support agent.</span></span>
