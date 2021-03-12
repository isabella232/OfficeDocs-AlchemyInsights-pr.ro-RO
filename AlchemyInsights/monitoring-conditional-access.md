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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708686"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="44dc2-102">Monitorizarea accesului condiționat pentru Exchange</span><span class="sxs-lookup"><span data-stu-id="44dc2-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="44dc2-103">Utilizatorii vizați de Access condițional vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="44dc2-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="44dc2-104">Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="44dc2-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="44dc2-105">Dacă se presupune că dispozitivul este înscris, consiliați utilizatorul să meargă la aplicația portal a firmei și să verifice dacă apare în portalul firmei.</span><span class="sxs-lookup"><span data-stu-id="44dc2-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="44dc2-106">Dacă nu, utilizatorul trebuie să înscrie dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="44dc2-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="44dc2-107">În portalul Azure, accesați Intune > conformitatea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="44dc2-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="44dc2-108">Sub monitor, faceți clic pe conformitate dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="44dc2-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="44dc2-109">Vizualizați raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca fiind conform.</span><span class="sxs-lookup"><span data-stu-id="44dc2-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="44dc2-110">În portalul Azure, accesați Intune > conformitatea dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="44dc2-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="44dc2-111">Sub gestionare, faceți clic pe politici.</span><span class="sxs-lookup"><span data-stu-id="44dc2-111">Under Manage, click Policies.</span></span> <span data-ttu-id="44dc2-112">În lista de politici de conformitate, Verificați dacă un profil este atribuit dispozitivului utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="44dc2-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="44dc2-113">Dacă nu este atribuit niciun profil, atunci Intune nu va putea confirma starea de conformitate a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="44dc2-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="44dc2-114">Editați atribuirea accesului condiționat al utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="44dc2-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="44dc2-115">În portalul Azure, accesați Politica de   >  **acces condițională** Intune  >  .</span><span class="sxs-lookup"><span data-stu-id="44dc2-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="44dc2-116">Selectați o politică din listă.</span><span class="sxs-lookup"><span data-stu-id="44dc2-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="44dc2-117">Faceți clic pe utilizatori și grupuri.</span><span class="sxs-lookup"><span data-stu-id="44dc2-117">Click Users and groups.</span></span>
4. <span data-ttu-id="44dc2-118">Pentru a viza o anumită politică la o persoană, adăugați-o la lista includere.</span><span class="sxs-lookup"><span data-stu-id="44dc2-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="44dc2-119">Pentru a vă asigura că o persoană este omisă din politică, adăugați-o la lista de excluderi.</span><span class="sxs-lookup"><span data-stu-id="44dc2-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="44dc2-120">Linkuri utile:</span><span class="sxs-lookup"><span data-stu-id="44dc2-120">Helpful links:</span></span>

[<span data-ttu-id="44dc2-121">Prezentare generală a conformității dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="44dc2-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="44dc2-122">Depanarea CA</span><span class="sxs-lookup"><span data-stu-id="44dc2-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="44dc2-123">Politica de depanare</span><span class="sxs-lookup"><span data-stu-id="44dc2-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="44dc2-124">Monitorizarea conformității dispozitivelor Intune</span><span class="sxs-lookup"><span data-stu-id="44dc2-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="44dc2-125">Notă: acești pași sunt utili doar în depanarea caracteristicii Azure Active Directory Access condiționale.</span><span class="sxs-lookup"><span data-stu-id="44dc2-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="44dc2-126">De asemenea, este posibil să plasați în carantină un dispozitiv care blochează accesul la e-mail cu politica Exchange.</span><span class="sxs-lookup"><span data-stu-id="44dc2-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="44dc2-127">Mai multe informații despre gestionarea dispozitivelor Exchange pot fi găsite [aici] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="44dc2-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
