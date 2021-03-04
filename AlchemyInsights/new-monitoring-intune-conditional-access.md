---
title: Monitorizarea accesului condițional al Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427927"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="45461-102">Monitorizarea accesului condițional al Intune</span><span class="sxs-lookup"><span data-stu-id="45461-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="45461-103">Utilizatorii vizați de Access condițional vor primi un e-mail de notificare dacă nu îndeplinesc cerințele de acces ale organizației dvs.</span><span class="sxs-lookup"><span data-stu-id="45461-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="45461-104">Pentru a rezolva, vă recomandăm una sau mai multe dintre următoarele soluții:</span><span class="sxs-lookup"><span data-stu-id="45461-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="45461-105">Dacă se presupune că dispozitivul este înscris, consiliați utilizatorul să meargă la aplicația portal a firmei și să verifice dacă apare în portalul firmei.</span><span class="sxs-lookup"><span data-stu-id="45461-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="45461-106">Dacă nu, utilizatorul trebuie să înscrie dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="45461-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="45461-107">În portalul Azure, accesați   >  **conformitatea dispozitivelor** Intune.</span><span class="sxs-lookup"><span data-stu-id="45461-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="45461-108">Pentru a vedea raportul de conformitate al dispozitivului pentru a verifica dacă dispozitivul utilizatorului este marcat ca fiind conform, sub **Monitor**, faceți clic pe **conformitate dispozitiv**.</span><span class="sxs-lookup"><span data-stu-id="45461-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="45461-109">În portalul Azure, accesați   >  **conformitatea dispozitivelor** Intune.</span><span class="sxs-lookup"><span data-stu-id="45461-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="45461-110">Sub **gestionare,** faceți clic pe **politici**.</span><span class="sxs-lookup"><span data-stu-id="45461-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="45461-111">În lista de politici de conformitate, Verificați dacă un profil este atribuit dispozitivului utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="45461-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="45461-112">Dacă nu este atribuit niciun profil, atunci Intune nu va putea confirma starea de conformitate a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="45461-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="45461-113">Editați atribuirea accesului condiționat al utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="45461-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="45461-114">În portalul Azure, navigați la politicile de   >  **acces condiționale** Intune  >  , selectați o politică din listă și faceți clic pe **utilizatori și grupuri**.</span><span class="sxs-lookup"><span data-stu-id="45461-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="45461-115">Pentru a viza o anumită politică la o persoană, adăugați-o la **lista includere**.</span><span class="sxs-lookup"><span data-stu-id="45461-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="45461-116">Pentru a vă asigura că o persoană este omisă din politică, adăugați-o la **lista de excluderi**.</span><span class="sxs-lookup"><span data-stu-id="45461-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="45461-117">**Linkuri utile:**</span><span class="sxs-lookup"><span data-stu-id="45461-117">**Helpful links:**</span></span>

- [<span data-ttu-id="45461-118">Prezentare generală a conformității dispozitivelor</span><span class="sxs-lookup"><span data-stu-id="45461-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="45461-119">Depanarea CA</span><span class="sxs-lookup"><span data-stu-id="45461-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="45461-120">Politica de depanare</span><span class="sxs-lookup"><span data-stu-id="45461-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="45461-121">Monitorizarea conformității dispozitivelor Intune</span><span class="sxs-lookup"><span data-stu-id="45461-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="45461-122">Acești pași sunt utili doar pentru depanarea caracteristicii Azure Active Directory Access condiționale.</span><span class="sxs-lookup"><span data-stu-id="45461-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="45461-123">De asemenea, este posibil să plasați în carantină un dispozitiv care blochează accesul la e-mail cu politica Exchange.</span><span class="sxs-lookup"><span data-stu-id="45461-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="45461-124">Mai multe informații despre gestionarea dispozitivelor Exchange pot fi găsite [**aici**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="45461-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
