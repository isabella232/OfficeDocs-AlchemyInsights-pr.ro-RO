---
title: Probleme de acces condiționat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014890"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="7f01b-102">Probleme de acces condiționat</span><span class="sxs-lookup"><span data-stu-id="7f01b-102">Conditional access issues</span></span>

<span data-ttu-id="7f01b-103">**Rezolvarea problemelor cu diagnosticul de conectare**</span><span class="sxs-lookup"><span data-stu-id="7f01b-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="7f01b-104">Puteți afla rapid ce s-a întâmplat sau cum să diagnosticați problemele legate de conectarea la utilizator, utilizând [diagnosticul de conectare](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="7f01b-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="7f01b-105">Lansați diagnosticul de conectare.</span><span class="sxs-lookup"><span data-stu-id="7f01b-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="7f01b-106">Găsiți evenimentul de analizat introducând detaliile pe care le aveți despre utilizator, aplicație, ora conectării, ID-ul de solicitare sau ID-ul de corelare.</span><span class="sxs-lookup"><span data-stu-id="7f01b-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="7f01b-107">Revizuiți rezultatele de diagnosticare care afișează detaliile despre ce s-a întâmplat și ce acțiuni puteți efectua pentru a face modificări (dacă sunt necesare modificări).</span><span class="sxs-lookup"><span data-stu-id="7f01b-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="7f01b-108">**Pașii pentru depanarea unui sign in**</span><span class="sxs-lookup"><span data-stu-id="7f01b-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="7f01b-109">Navigați la pagina de conectare la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f01b-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="7f01b-110">Filtrați sign-in-uri după utilizator, interval de timp, aplicație, stare, aplicație client etc.</span><span class="sxs-lookup"><span data-stu-id="7f01b-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="7f01b-111">Selectați un eveniment de conectare și vizualizați fila acces condiționat pentru a vedea ce politici au fost evaluate.</span><span class="sxs-lookup"><span data-stu-id="7f01b-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="7f01b-112">Faceți clic pe rândul unei politici pentru a vizualiza detaliile politicii și a înțelege de ce s-a aplicat.</span><span class="sxs-lookup"><span data-stu-id="7f01b-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="7f01b-113">**Instrumente pentru a depana o politică de acces condiționat**</span><span class="sxs-lookup"><span data-stu-id="7f01b-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="7f01b-114">Modul doar în raport vă permite să evaluați o politică fără a afecta utilizatorii.</span><span class="sxs-lookup"><span data-stu-id="7f01b-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="7f01b-115">Instrumentul ce-If vă permite să simulați evenimentele de conectare și să vedeți ce politici se aplică.</span><span class="sxs-lookup"><span data-stu-id="7f01b-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="7f01b-116">Detalii și registru de lucru raportare afișează impactul în timp real al fiecărei politici.</span><span class="sxs-lookup"><span data-stu-id="7f01b-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="7f01b-117">**Politici de protecție de referință**</span><span class="sxs-lookup"><span data-stu-id="7f01b-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="7f01b-118">Politicile de protecție de referință au fost dezaprobate.</span><span class="sxs-lookup"><span data-stu-id="7f01b-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="7f01b-119">Acestea nu mai sunt impuse și vor fi eliminate în curând din portalul Azure.</span><span class="sxs-lookup"><span data-stu-id="7f01b-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="7f01b-120">Vă recomandăm să activați [valorile implicite de securitate](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="7f01b-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="7f01b-121">Pentru mai multe informații despre accesul condiționat, consultați:</span><span class="sxs-lookup"><span data-stu-id="7f01b-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="7f01b-122">[Cele mai bune practici pentru accesul condiționat din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condiții în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controale în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locații în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="7f01b-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
