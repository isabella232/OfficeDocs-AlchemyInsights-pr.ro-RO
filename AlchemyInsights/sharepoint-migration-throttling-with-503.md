---
title: Migrare SharePoint limitare cu 503 erori
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931670"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="a5f40-102">Migrare SharePoint limitare cu 503 erori</span><span class="sxs-lookup"><span data-stu-id="a5f40-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="a5f40-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="a5f40-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a5f40-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="a5f40-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a5f40-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="a5f40-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a5f40-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="a5f40-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a5f40-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="a5f40-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a5f40-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="a5f40-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a5f40-109">**503 erori la migrarea la SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="a5f40-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="a5f40-110">Se pare că migrați la SharePoint Online și primiți 503 erori.</span><span class="sxs-lookup"><span data-stu-id="a5f40-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="a5f40-111">Vă rugăm să urmați pașii de mai jos, astfel încât să vă putem ajuta cât mai curând posibil.</span><span class="sxs-lookup"><span data-stu-id="a5f40-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="a5f40-112">Faceți clic pe **Contact Support**, apoi pe Solicitare **serviciu nou**.</span><span class="sxs-lookup"><span data-stu-id="a5f40-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="a5f40-113">Pentru titlu și descriere, tastați **Throttling migrare SharePoint cu 503**.</span><span class="sxs-lookup"><span data-stu-id="a5f40-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="a5f40-114">După ce biletul a fost remis, vă rugăm să îl actualizați cu următoarele informații:</span><span class="sxs-lookup"><span data-stu-id="a5f40-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="a5f40-115">Cât de mult a mai rămas din migrație (de exemplu, cât de multe TBs?).</span><span class="sxs-lookup"><span data-stu-id="a5f40-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="a5f40-116">Data de început și de sfârșit a migrării.</span><span class="sxs-lookup"><span data-stu-id="a5f40-116">Migration start and end date.</span></span>
    - <span data-ttu-id="a5f40-117">Descrieți de unde migrați conținutul, ar fi SharePoint Server, Box, GDrive, Partajări de fișiere etc..</span><span class="sxs-lookup"><span data-stu-id="a5f40-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="a5f40-118">Estimați numărul de erori de limitare (de exemplu, x accelerație pe oră?) și când s-a întâmplat limitarea.</span><span class="sxs-lookup"><span data-stu-id="a5f40-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="a5f40-119">Ce instrument de migrare utilizați (de exemplu, SPMT sau ShareGate).</span><span class="sxs-lookup"><span data-stu-id="a5f40-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


