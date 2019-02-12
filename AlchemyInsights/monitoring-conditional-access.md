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
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902370"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="a61ca-102">Monitorizare acces condiționat</span><span class="sxs-lookup"><span data-stu-id="a61ca-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="a61ca-p101">Utilizatorii orientate cu acces condiționat vor primi un e-mail de notificare, în cazul în care nu îndeplinesc cerinţele de acces al organizaţiei. Pentru a rezolva, va recomandam unul sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="a61ca-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a61ca-p102">În cazul în care dispozitivul este prezumată a fi înscrişi, sfătui utilizatorul să accesaţi aplicaţia Portal de companie şi să verifice că acesta apare în portalul companiei. Dacă nu, utilizatorul ar trebui să înscrieţi-vă dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="a61ca-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a61ca-p103">În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**. Sub **monitorul de** faceţi clic pe **dispozitiv conformitatea**. Vezi dispozitiv conformitatea raport pentru a verifica că utilizatorul final este marcat ca conforme.</span><span class="sxs-lookup"><span data-stu-id="a61ca-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a61ca-p104">În portalul azuriu Du-te la **Intune \> dispozitiv respectarea**. La **administrare**, faceţi clic pe **politici**. În lista de conformitatea politicilor, verificaţi că un profil este atribuit de utilizator pe dispozitiv. Dacă este alocat nici un profil, apoi Intune nu va fi capabil să confirme statutul de conformitatea dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="a61ca-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a61ca-114">Editare cesiune de acces condiționat utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="a61ca-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a61ca-115">În portalul azuriu Du-te la **Intune \> acces condiţionat \> politici**</span><span class="sxs-lookup"><span data-stu-id="a61ca-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a61ca-116">Selectaţi o politică din lista</span><span class="sxs-lookup"><span data-stu-id="a61ca-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a61ca-117">Faceţi clic pe **utilizatori și grupuri**</span><span class="sxs-lookup"><span data-stu-id="a61ca-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a61ca-p105">Pentru a-ţintă o anumită politică la cineva, adăugaţi-le la lista de **includeri** . Pentru a se asigura că o persoană este omis din politica, adăugaţi-le la lista de **Exclude** .</span><span class="sxs-lookup"><span data-stu-id="a61ca-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a61ca-120">Citeşte mai departe: [modul de acces condiționat Monitor dispozitive](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a61ca-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

