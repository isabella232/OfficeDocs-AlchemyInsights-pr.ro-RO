---
title: Faceți descoperirea site-ului
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694560"
---
# <a name="do-site-discovery"></a><span data-ttu-id="0e88c-102">Faceți descoperirea site-ului</span><span class="sxs-lookup"><span data-stu-id="0e88c-102">Do site discovery</span></span>

<span data-ttu-id="0e88c-103">Dacă organizația utilizează încă aplicații web moștenite și intenționează să utilizeze modul Internet Explorer (pe care o fac majoritatea clienților), ar trebui să efectuați o descoperire suplimentară a site-ului.</span><span class="sxs-lookup"><span data-stu-id="0e88c-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="0e88c-104">**Ați implementat deja o versiune mai veche de Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="0e88c-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="0e88c-105">Dacă ați configurat deja lista de site-uri de întreprindere pentru a lucra pentru versiunea moștenită de Microsoft Edge, atunci descoperirea site-ului este aproape gata.</span><span class="sxs-lookup"><span data-stu-id="0e88c-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="0e88c-106">Singurul lucru pe care ar trebui să-l faceți este să adăugați site-uri neutre.</span><span class="sxs-lookup"><span data-stu-id="0e88c-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="0e88c-107">Site-urile neutre sunt de obicei site-uri care furnizează sign-on unic (SSO).</span><span class="sxs-lookup"><span data-stu-id="0e88c-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="0e88c-108">Dacă accesați un site neutru din Microsoft Edge, atunci doriți să rămâneți în Microsoft Edge pentru a vă autentifica.</span><span class="sxs-lookup"><span data-stu-id="0e88c-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="0e88c-109">Dacă accesați un site neutru în modul Internet Explorer, atunci doriți să rămâneți în modul Internet Explorer pentru a vă autentifica.</span><span class="sxs-lookup"><span data-stu-id="0e88c-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="0e88c-110">Identificați orice SSO sau alte site-uri neutre pe care le utilizați și adăugați-le în lista de site-uri de întreprindere.</span><span class="sxs-lookup"><span data-stu-id="0e88c-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="0e88c-111">**Internet Explorer este browserul implicit**</span><span class="sxs-lookup"><span data-stu-id="0e88c-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="0e88c-112">Dacă utilizați acum Internet Explorer, este posibil să nu știți ce site-uri au făcut upgrade la standardele web moderne și care necesită încă Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0e88c-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="0e88c-113">Veți dori să găsiți și să adăugați aceste site-uri la lista site-ului de întreprindere, astfel încât să puteți utiliza modul Internet Explorer doar pentru acele site-uri.</span><span class="sxs-lookup"><span data-stu-id="0e88c-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="0e88c-114">[Descoperirea site-ului Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) descoperă site-uri care pot necesita modul Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0e88c-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="0e88c-115">Poate colecta date pe computerele care execută Windows Internet Explorer 8 prin Internet Explorer 11 în Windows 10, Windows 8,1 sau Windows 7.</span><span class="sxs-lookup"><span data-stu-id="0e88c-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="0e88c-116">**Analizarea datelor**</span><span class="sxs-lookup"><span data-stu-id="0e88c-116">**Analyze the data**</span></span>

<span data-ttu-id="0e88c-117">După ce ați colectat datele de site, vă recomandăm următorul proces în patru pași pentru a analiza datele:</span><span class="sxs-lookup"><span data-stu-id="0e88c-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="0e88c-118">Sortați datele după domeniu, apoi după URL.</span><span class="sxs-lookup"><span data-stu-id="0e88c-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="0e88c-119">Definiți limitele unei aplicații pentru a configura modul Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0e88c-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="0e88c-120">Doriți să includeți toate site-urile și controalele web care definesc aplicația, dar nu doriți să includeți site-uri și controale suplimentare.</span><span class="sxs-lookup"><span data-stu-id="0e88c-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="0e88c-121">Unele site-uri pot fi la fel de simple ca *https://contoso.com/app1* în timp ce alte persoane vă pot solicita să definiți mai multe site-uri și pagini.</span><span class="sxs-lookup"><span data-stu-id="0e88c-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="0e88c-122">Testați aplicația pentru a verifica dacă nu funcționează în mod nativ.</span><span class="sxs-lookup"><span data-stu-id="0e88c-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="0e88c-123">Multe site-uri vor oferi conținut modern atunci când detectează un browser modern și oferă doar conținut moștenit atunci când detectează Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0e88c-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="0e88c-124">Adăugați aplicația la lista de site-uri de întreprindere dacă nu reușește testarea.</span><span class="sxs-lookup"><span data-stu-id="0e88c-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="0e88c-125">Ca o practică optimă, grupați toate site-urile care cuprind o aplicație.</span><span class="sxs-lookup"><span data-stu-id="0e88c-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="0e88c-126">În acest fel, atunci când faceți upgrade unei aplicații, este mai ușor să eliminați întregul site din modul Internet Explorer și să începeți să utilizați un browser modern pentru acea aplicație.</span><span class="sxs-lookup"><span data-stu-id="0e88c-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="0e88c-127">După ce ați terminat cu descoperirea site-ului și ați analizat datele, sunteți gata să începeți să vă uitați la strategia de canal.</span><span class="sxs-lookup"><span data-stu-id="0e88c-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

