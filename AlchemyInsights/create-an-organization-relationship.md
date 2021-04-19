---
title: Crearea unei relații de organizație pentru a le permite utilizatorilor să colaboreze cu altă organizație
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816140"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="41f61-102">Crearea unei relații de organizație pentru a le permite utilizatorilor să colaboreze cu altă organizație</span><span class="sxs-lookup"><span data-stu-id="41f61-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="41f61-103">Din tabloul de bord al centrului de administrare Microsoft 365, accesați **Admin**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="41f61-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="41f61-104">Accesați **partajarea**  >  **organizației.**</span><span class="sxs-lookup"><span data-stu-id="41f61-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="41f61-105">Sub Partajare **organizație, faceți** clic **pe Nou** .</span><span class="sxs-lookup"><span data-stu-id="41f61-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="41f61-106">În **noua relație de organizație,** în caseta Nume **relație,** tastați un nume prietenos pentru relația organizației.</span><span class="sxs-lookup"><span data-stu-id="41f61-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="41f61-107">În caseta **Domenii** de partajat cu, tastați domeniul pentru organizația office 365 sau Exchange externă pe care doriți să o permiteți să vedeți calendarele.</span><span class="sxs-lookup"><span data-stu-id="41f61-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="41f61-108">Dacă trebuie să introduceți mai multe domenii, separați numele de domeniu prin virgulă.</span><span class="sxs-lookup"><span data-stu-id="41f61-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="41f61-109">De exemplu, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="41f61-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="41f61-110">Bifați caseta **de selectare Activați partajarea informațiilor liber/ocupat** din calendar pentru a activa partajarea calendarelor cu domeniile listate.</span><span class="sxs-lookup"><span data-stu-id="41f61-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="41f61-111">Setați nivelul de partajare pentru informațiile liber/ocupat din calendar și setați ce utilizatori pot partaja informațiile liber/ocupat din calendar.</span><span class="sxs-lookup"><span data-stu-id="41f61-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="41f61-112">Pentru a seta nivelul de acces liber/ocupat, selectați una dintre următoarele:</span><span class="sxs-lookup"><span data-stu-id="41f61-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="41f61-113">**Informații liber/ocupat din calendar doar cu timpul**</span><span class="sxs-lookup"><span data-stu-id="41f61-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="41f61-114">**Liber/ocupat din calendar cu timpul, subiectul și locația**</span><span class="sxs-lookup"><span data-stu-id="41f61-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="41f61-115">Pentru a seta utilizatorii care vor partaja informații liber/ocupat din calendar, selectați una dintre următoarele:</span><span class="sxs-lookup"><span data-stu-id="41f61-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="41f61-116">**Toate persoanele din organizația dvs.**</span><span class="sxs-lookup"><span data-stu-id="41f61-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="41f61-117">**Un grup de securitate specificat**</span><span class="sxs-lookup"><span data-stu-id="41f61-117">**A specified security group**</span></span>  

<span data-ttu-id="41f61-118">Faceți **clic** pe răsfoire pentru a alege grupul de securitate dintr-o listă, apoi faceți clic **pe OK.**</span><span class="sxs-lookup"><span data-stu-id="41f61-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="41f61-119">Faceți **clic** pe salvare pentru a crea relația de organizație.</span><span class="sxs-lookup"><span data-stu-id="41f61-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="41f61-120">**Notă:** Configurațiile între entități găzduite nu acceptă persoanele de contact personale pentru căutare liber/ocupat.</span><span class="sxs-lookup"><span data-stu-id="41f61-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="41f61-121">Persoanele de contact trebuie să fie incluse în lista globală de adrese pentru ca căutare liber/ocupat să lucreze.</span><span class="sxs-lookup"><span data-stu-id="41f61-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="41f61-122">**Pentru a înțelege complet acest subiect, citiți:**</span><span class="sxs-lookup"><span data-stu-id="41f61-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="41f61-123">Crearea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="41f61-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="41f61-124">Modificarea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="41f61-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="41f61-125">Eliminarea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="41f61-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
