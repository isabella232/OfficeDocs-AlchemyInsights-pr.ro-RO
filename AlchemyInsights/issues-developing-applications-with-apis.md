---
title: Probleme cu dezvoltarea aplicațiilor cu API-uri
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975015"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="b132f-102">Probleme cu dezvoltarea aplicațiilor cu API-uri</span><span class="sxs-lookup"><span data-stu-id="b132f-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="b132f-103">Pentru a începe să utilizați API-ul Azure Active Directory Graph, consultați [Ghidul de pornire rapidă AZURE AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) sau vizualizați [documentația de referințe interactive AZURE AD Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="b132f-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="b132f-104">**Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="b132f-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="b132f-105">**Începând cu 30 iunie 2020**, nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b132f-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="b132f-106">Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.</span><span class="sxs-lookup"><span data-stu-id="b132f-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="b132f-107">**Începând cu 30 iunie, 2022**, vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="b132f-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="b132f-108">Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi nicio asistență tehnică sau actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="b132f-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="b132f-109">Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b132f-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="b132f-110">**Migrarea monica**</span><span class="sxs-lookup"><span data-stu-id="b132f-110">**ADAL Migration**</span></span>

<span data-ttu-id="b132f-111">Vă recomandăm să actualizați la [biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="b132f-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="b132f-112">Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, pentru a se asigura că va beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.</span><span class="sxs-lookup"><span data-stu-id="b132f-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="b132f-113">[Citiți întrebările frecvente](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)despre Monica.</span><span class="sxs-lookup"><span data-stu-id="b132f-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="b132f-114">[Aflați cum să migrați aplicațiile pe o bază per platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="b132f-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="b132f-115">Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații.</span><span class="sxs-lookup"><span data-stu-id="b132f-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b132f-116">Asistența Microsoft vă poate oferi, de asemenea, o listă cu toate aplicațiile non-Microsoft Monica din entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="b132f-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="b132f-117">**Migrarea graficului AAD**</span><span class="sxs-lookup"><span data-stu-id="b132f-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="b132f-118">Pentru aplicațiile care utilizează Azure AD Graph, urmați ghidul nostru pentru a migra [aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b132f-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="b132f-119">[Lista de verificare a migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="b132f-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="b132f-120">Portalul de înregistrare Azure App Arată ce aplicații utilizează Dan Graph.</span><span class="sxs-lookup"><span data-stu-id="b132f-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="b132f-121">Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații.</span><span class="sxs-lookup"><span data-stu-id="b132f-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b132f-122">Asistența Microsoft vă poate oferi, de asemenea, o listă cu utilizarea tuturor grafurilor în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="b132f-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="b132f-123">Pentru ca aplicația să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să îi acorde permisiunile corecte printr-un proces de consimțământ.</span><span class="sxs-lookup"><span data-stu-id="b132f-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="b132f-124">[Referințele pentru permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) listează permisiunile asociate cu fiecare set principal de API-uri Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b132f-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="b132f-125">De asemenea, furnizează instrucțiuni despre cum se utilizează permisiunile.</span><span class="sxs-lookup"><span data-stu-id="b132f-125">It also provides guidance about how to use the permissions.</span></span>
