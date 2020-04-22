---
title: Monitorizarea accesului condiționat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713730"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="53a7e-102">Monitorizarea accesului condiționat pentru exchange</span><span class="sxs-lookup"><span data-stu-id="53a7e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="53a7e-103">Utilizatorii vizați cu acces condiționat vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="53a7e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="53a7e-104">Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="53a7e-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="53a7e-105">Dacă se presupune că dispozitivul este înscris, sfătuiți utilizatorul să meargă la aplicația Portal companie și verificați dacă apare în portalul companiei.</span><span class="sxs-lookup"><span data-stu-id="53a7e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="53a7e-106">Dacă nu, utilizatorul ar trebui să înscrie dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="53a7e-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="53a7e-107">În portalul Azure accesați **Intune \> dispozitiv conformitate**.</span><span class="sxs-lookup"><span data-stu-id="53a7e-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="53a7e-108">Sub **Monitor,** faceți clic pe **Conformitate dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="53a7e-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="53a7e-109">Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca compatibil.</span><span class="sxs-lookup"><span data-stu-id="53a7e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="53a7e-110">În portalul Azure accesați **Intune \> dispozitiv conformitate**.</span><span class="sxs-lookup"><span data-stu-id="53a7e-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="53a7e-111">Sub **Gestionare**, faceți clic pe **Politici**.</span><span class="sxs-lookup"><span data-stu-id="53a7e-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="53a7e-112">În lista de politici de conformitate, verificați dacă un profil este atribuit dispozitivului utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="53a7e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="53a7e-113">Dacă nu este atribuit niciun profil, Intune nu va putea confirma starea de conformitate a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="53a7e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="53a7e-114">Editați atribuirea de acces condiționat a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="53a7e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="53a7e-115">În portalul Azure accesați \*\* \> Intune \> condițională accesați politicile de acces\*\*</span><span class="sxs-lookup"><span data-stu-id="53a7e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="53a7e-116">Selectarea unei politici din listă</span><span class="sxs-lookup"><span data-stu-id="53a7e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="53a7e-117">Faceți clic pe **Utilizatori și grupuri**</span><span class="sxs-lookup"><span data-stu-id="53a7e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="53a7e-118">Pentru a viza o anumită politică către o persoană, adăugați-le în lista **Includere.**</span><span class="sxs-lookup"><span data-stu-id="53a7e-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="53a7e-119">Pentru a vă asigura că o persoană este omisă din politică, adăugați-le la lista **Excludere.**</span><span class="sxs-lookup"><span data-stu-id="53a7e-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="53a7e-120">Citiți mai mult: [Cum se monitorizează dispozitivele de acces condiționat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="53a7e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

