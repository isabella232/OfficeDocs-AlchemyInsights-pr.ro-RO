---
title: Probleme cu dezvoltarea aplicațiilor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974770"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="5378f-102">Probleme cu dezvoltarea aplicațiilor</span><span class="sxs-lookup"><span data-stu-id="5378f-102">Issues developing applications</span></span>

<span data-ttu-id="5378f-103">Pentru a depana problemele cele mai comune atunci când construiți aplicații Azure Active Directory (AD), consultați următoarele articole:</span><span class="sxs-lookup"><span data-stu-id="5378f-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="5378f-104">Văd probleme la conectarea la aplicații folosind doar browserul Chrome</span><span class="sxs-lookup"><span data-stu-id="5378f-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="5378f-105">Nu știu cum să modific valorile implicite pentru durata de viață a tokenului pentru aplicația mea</span><span class="sxs-lookup"><span data-stu-id="5378f-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="5378f-106">Sunt confuz în legătură cu modul în care funcționează consimțământul aplicației</span><span class="sxs-lookup"><span data-stu-id="5378f-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="5378f-107">Nu știu cum să acord permisiuni aplicației mele</span><span class="sxs-lookup"><span data-stu-id="5378f-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="5378f-108">Nu înțeleg diferența dintre permisiunile delegate și aplicație</span><span class="sxs-lookup"><span data-stu-id="5378f-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="5378f-109">\***Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și AZURE AD Graph API (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="5378f-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="5378f-110">Începând cu 30 iunie, 2020, nu vom mai adăuga caracteristici noi la Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="5378f-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="5378f-111">Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.</span><span class="sxs-lookup"><span data-stu-id="5378f-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="5378f-112">Începând cu 30 iunie, 2022, vom încheia suportul pentru monica și Dan grafic și nu va mai furniza asistență tehnică sau actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="5378f-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="5378f-113">Ca rezultat al acestei condiții, sunt implicați următoarele:</span><span class="sxs-lookup"><span data-stu-id="5378f-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="5378f-114">Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi nicio asistență tehnică sau actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="5378f-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="5378f-115">Este posibil ca aplicațiile care utilizează Dan Graph să nu mai primească răspunsuri de la punctul final din punct grafic</span><span class="sxs-lookup"><span data-stu-id="5378f-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="5378f-116">-*Migrarea* monica\*</span><span class="sxs-lookup"><span data-stu-id="5378f-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="5378f-117">Dacă utilizați aplicațiile Microsoft, vă recomandăm să actualizați la biblioteca de autentificare Microsoft (MSAL), care are cele mai recente caracteristici și actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="5378f-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="5378f-118">Această recomandare este în contextul Microsoft inițiază procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței.</span><span class="sxs-lookup"><span data-stu-id="5378f-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="5378f-119">Migrarea de la Microsoft a aplicațiilor sale către MSAL asigură faptul că aplicațiile beneficiază de îmbunătățiri de securitate și caracteristici ale MSAL.</span><span class="sxs-lookup"><span data-stu-id="5378f-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="5378f-120">Citiți întrebări frecvente despre Monica</span><span class="sxs-lookup"><span data-stu-id="5378f-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="5378f-121">Aflați cum să migrați aplicațiile pe o bază per platformă</span><span class="sxs-lookup"><span data-stu-id="5378f-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="5378f-122">Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să luați legătura cu orice vânzători de software independenți (ISV) sau furnizori de aplicații.</span><span class="sxs-lookup"><span data-stu-id="5378f-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="5378f-123">Asistența Microsoft vă poate oferi, de asemenea, o listă cu toate aplicațiile non-Microsoft Monica din entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="5378f-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="5378f-124">**Migrarea graficului AAD**</span><span class="sxs-lookup"><span data-stu-id="5378f-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="5378f-125">Pentru aplicațiile care utilizează Dan Graph, urmați ghidul nostru pentru a migra aplicațiile cu un grafic AAD la Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="5378f-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="5378f-126">[Lista de verificare a migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="5378f-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="5378f-127">Portalul de înregistrare Azure App Arată ce aplicații utilizează Dan Graph.</span><span class="sxs-lookup"><span data-stu-id="5378f-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="5378f-128">Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați vânzătorii de software independenți (ISV) sau furnizorii de aplicații.</span><span class="sxs-lookup"><span data-stu-id="5378f-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="5378f-129">Asistența Microsoft vă poate oferi, de asemenea, informații despre utilizarea în Graph a graficului în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="5378f-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







