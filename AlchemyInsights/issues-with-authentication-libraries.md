---
title: Probleme cu bibliotecile de autentificare
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063642"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="19e93-102">Probleme cu bibliotecile de autentificare</span><span class="sxs-lookup"><span data-stu-id="19e93-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="19e93-103">[Bibliotecile de autentificare a platformelor Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listează bibliotecile client și middleware compatibile Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19e93-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="19e93-104">Biblioteca de autentificare Microsoft (MSAL) acceptă mai multe [fluxuri de autentificare](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) pentru utilizare în scenarii de aplicație diferite.</span><span class="sxs-lookup"><span data-stu-id="19e93-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="19e93-105">Pentru a autentifica și a achiziționa jetoane, inițializați o nouă aplicație publică sau confidențială pentru clientul dumneavoastră în cod.</span><span class="sxs-lookup"><span data-stu-id="19e93-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="19e93-106">Puteți seta mai multe opțiuni de configurare atunci când inițializați aplicația client în biblioteca de autentificare Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="19e93-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="19e93-107">Pentru a afla mai multe, consultați [opțiunile de configurare a aplicațiilor](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="19e93-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="19e93-108">**Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="19e93-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="19e93-109">**Începând cu 30 iunie 2020**, nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="19e93-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="19e93-110">Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.</span><span class="sxs-lookup"><span data-stu-id="19e93-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="19e93-111">**Începând cu 30 iunie, 2022**, vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="19e93-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="19e93-112">Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor *primi nicio asistență tehnică sau actualizări de securitate*.</span><span class="sxs-lookup"><span data-stu-id="19e93-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="19e93-113">Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="19e93-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="19e93-114">**Migrarea monica**</span><span class="sxs-lookup"><span data-stu-id="19e93-114">**ADAL Migration**</span></span>

<span data-ttu-id="19e93-115">Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate.</span><span class="sxs-lookup"><span data-stu-id="19e93-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="19e93-116">Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, asigurându-vă că acestea vor beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.</span><span class="sxs-lookup"><span data-stu-id="19e93-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="19e93-117">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="19e93-117">For more information, see:</span></span>

1. [<span data-ttu-id="19e93-118">Citiți întrebările frecvente despre ADAL</span><span class="sxs-lookup"><span data-stu-id="19e93-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="19e93-119">Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă</span><span class="sxs-lookup"><span data-stu-id="19e93-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="19e93-120">Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații.</span><span class="sxs-lookup"><span data-stu-id="19e93-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="19e93-121">De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="19e93-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="19e93-122">**Migrarea AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="19e93-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="19e93-123">Pentru aplicațiile care utilizează Azure AD Graph, urmați ghidul nostru pentru a [migra aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="19e93-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="19e93-124">Lista de verificare a migrării oferă un punct de pornire.</span><span class="sxs-lookup"><span data-stu-id="19e93-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="19e93-125">Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="19e93-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="19e93-126">Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații.</span><span class="sxs-lookup"><span data-stu-id="19e93-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="19e93-127">Asistența Microsoft vă poate oferi, de asemenea, o listă cu utilizarea tuturor grafurilor în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="19e93-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="19e93-128">Pentru ca aplicația să acceseze date în Microsoft Graph, utilizatorul sau administratorul trebuie să îi acorde permisiunile corecte printr-un proces de consimțământ.</span><span class="sxs-lookup"><span data-stu-id="19e93-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="19e93-129">[Referințele pentru permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) listează permisiunile asociate cu fiecare set principal de API-uri Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="19e93-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="19e93-130">De asemenea, furnizează instrucțiuni despre cum se utilizează permisiunile.</span><span class="sxs-lookup"><span data-stu-id="19e93-130">It also provides guidance about how to use the permissions.</span></span>
