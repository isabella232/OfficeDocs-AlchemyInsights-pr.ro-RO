---
title: Dlp Politica Sfaturi nu funcționează
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932598"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="10091-102">Probleme cu vârful de politică DLP</span><span class="sxs-lookup"><span data-stu-id="10091-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="10091-103">**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal.</span><span class="sxs-lookup"><span data-stu-id="10091-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="10091-104">Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă.</span><span class="sxs-lookup"><span data-stu-id="10091-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="10091-105">În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="10091-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="10091-106">În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii.</span><span class="sxs-lookup"><span data-stu-id="10091-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="10091-107">Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade.</span><span class="sxs-lookup"><span data-stu-id="10091-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="10091-108">Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.</span><span class="sxs-lookup"><span data-stu-id="10091-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="10091-109">**Sfaturi de politică DLP**</span><span class="sxs-lookup"><span data-stu-id="10091-109">**DLP policy tips**</span></span>

<span data-ttu-id="10091-110">Când se **utilizează politici DLP**, utilizatorii pot fi notificați cu privire la o încălcare a politicii cu **sfaturi de politică**.</span><span class="sxs-lookup"><span data-stu-id="10091-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="10091-111">Administratorii pot configura sfaturi de politică pentru a afișa în timp ce testează politica DLP sau atunci când politica este în modul de aplicare completă.</span><span class="sxs-lookup"><span data-stu-id="10091-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="10091-112">Pentru a configura sfaturi de politică privind politica DLP în centrul de securitate și conformitate în modul de aplicare completă, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="10091-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="10091-113">Asigurați-vă că sfaturile de **politică** au fost activate pe regula DLP utilizând pașii [de aici](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="10091-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="10091-114">Asigurați-vă că **conținutul corespunde cu** ceea ce este **necesar** pentru a declanșa regula descrisă în acest articol [aici](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="10091-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="10091-115">Sfaturi de politică se afișează atât în OWA, cât și în Outlook.</span><span class="sxs-lookup"><span data-stu-id="10091-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="10091-116">Cu toate acestea, atunci când se utilizează **Outlook 2013 sau o versiune ulterioară**, sfaturi de politică sunt afișate numai în anumite condiții.</span><span class="sxs-lookup"><span data-stu-id="10091-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="10091-117">Aceste condiții sunt listate aici: [condiții acceptate pentru Outlook 2013 sau o versiune ulterioară pentru afișarea sfaturilor de politică](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="10091-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="10091-118">Pentru informații suplimentare despre sfaturile de politică DLP, consultați: [Afișare sfaturi de politică pentru politicile DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="10091-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  