---
title: Monitorizarea accesului condiționat
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702915"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="bb683-102">Monitorizarea accesului condiționat pentru Exchange</span><span class="sxs-lookup"><span data-stu-id="bb683-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="bb683-103">Utilizatorii vizați de Access condițional vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="bb683-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="bb683-104">Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="bb683-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bb683-105">Dacă se presupune că dispozitivul este înscris, consiliați utilizatorul să meargă la aplicația portal a firmei și să verifice dacă apare în portalul firmei.</span><span class="sxs-lookup"><span data-stu-id="bb683-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="bb683-106">Dacă nu, utilizatorul trebuie să înscrie dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="bb683-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bb683-107">În portalul Azure, accesați \*\* \> conformitatea dispozitivelor Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="bb683-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bb683-108">Sub **Monitor** , faceți clic pe **conformitate dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="bb683-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="bb683-109">Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca fiind conform.</span><span class="sxs-lookup"><span data-stu-id="bb683-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bb683-110">În portalul Azure, accesați \*\* \> conformitatea dispozitivelor Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="bb683-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bb683-111">Sub **gestionare**, faceți clic pe **politici**.</span><span class="sxs-lookup"><span data-stu-id="bb683-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="bb683-112">În lista de politici de conformitate, Verificați dacă un profil este atribuit dispozitivului utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="bb683-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="bb683-113">Dacă nu este atribuit niciun profil, atunci Intune nu va putea confirma starea de conformitate a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="bb683-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bb683-114">Editați atribuirea accesului condiționat al utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="bb683-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bb683-115">În portalul Azure accesați politicile de \*\* \> acces condiționale \> Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="bb683-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bb683-116">Selectați o politică din listă</span><span class="sxs-lookup"><span data-stu-id="bb683-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bb683-117">Faceți clic pe **utilizatori și grupuri**</span><span class="sxs-lookup"><span data-stu-id="bb683-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bb683-118">Pentru a viza o anumită politică la o persoană, adăugați-o la lista **Includere** .</span><span class="sxs-lookup"><span data-stu-id="bb683-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="bb683-119">Pentru a vă asigura că o persoană este omisă din politică, adăugați-o la lista de **excluderi** .</span><span class="sxs-lookup"><span data-stu-id="bb683-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bb683-120">Citiți mai mult: [cum să monitorizați dispozitivele de acces condiționat](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bb683-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

