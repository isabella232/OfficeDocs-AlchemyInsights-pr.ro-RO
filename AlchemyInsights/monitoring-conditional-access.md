---
title: Monitorizare acces condiționat
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538777"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e48fb-102">Monitorizare acces condiționat pentru schimb</span><span class="sxs-lookup"><span data-stu-id="e48fb-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e48fb-103">Utilizatorii orientate cu acces condiționat vor primi un e-mail de notificare, în cazul în care nu îndeplinesc cerinţele de acces al organizaţiei.</span><span class="sxs-lookup"><span data-stu-id="e48fb-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e48fb-104">Pentru a rezolva, va recomandam unul sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="e48fb-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e48fb-105">În cazul în care dispozitivul este prezumată a fi înscrişi, sfătui utilizatorul să accesaţi aplicaţia Portal de companie şi să verifice că acesta apare în portalul companiei.</span><span class="sxs-lookup"><span data-stu-id="e48fb-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e48fb-106">Dacă nu, utilizatorul ar trebui să înscrieţi-vă dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="e48fb-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e48fb-107">În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**.</span><span class="sxs-lookup"><span data-stu-id="e48fb-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e48fb-108">Sub **monitorul de** faceţi clic pe **dispozitiv conformitatea**.</span><span class="sxs-lookup"><span data-stu-id="e48fb-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e48fb-109">Vezi dispozitiv conformitatea raport pentru a verifica că utilizatorul final este marcat ca conforme.</span><span class="sxs-lookup"><span data-stu-id="e48fb-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e48fb-110">În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**.</span><span class="sxs-lookup"><span data-stu-id="e48fb-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e48fb-111">La **administrare**, faceţi clic pe **politici**.</span><span class="sxs-lookup"><span data-stu-id="e48fb-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e48fb-112">În lista de conformitatea politicilor, verificaţi că un profil este atribuit de utilizator pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="e48fb-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e48fb-113">Dacă este alocat nici un profil, apoi Intune nu va fi capabil să confirme statutul de conformitatea dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="e48fb-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e48fb-114">Editare cesiune de acces condiționat utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="e48fb-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e48fb-115">În portalul azuriu Du-te la **Intune \> acces condiţionat \> politici**</span><span class="sxs-lookup"><span data-stu-id="e48fb-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e48fb-116">Selectaţi o politică din lista</span><span class="sxs-lookup"><span data-stu-id="e48fb-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e48fb-117">Faceţi clic pe **utilizatori și grupuri**</span><span class="sxs-lookup"><span data-stu-id="e48fb-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e48fb-118">Pentru a-ţintă o anumită politică la cineva, adăugaţi-le la lista de **includeri** .</span><span class="sxs-lookup"><span data-stu-id="e48fb-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e48fb-119">Pentru a se asigura că o persoană este omis din politica, adăugaţi-le la lista de **Exclude** .</span><span class="sxs-lookup"><span data-stu-id="e48fb-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e48fb-120">Citeşte mai departe: [modul de acces condiționat Monitor dispozitive](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e48fb-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

