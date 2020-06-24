---
title: Crearea unei relații de organizație pentru a permite utilizatorilor să colaboreze cu altă organizație
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862196"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="38eb8-102">Crearea unei relații de organizație pentru a permite utilizatorilor să colaboreze cu altă organizație</span><span class="sxs-lookup"><span data-stu-id="38eb8-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="38eb8-103">Din tabloul de bord al centrului **Admin**de administrare Microsoft 365, accesați  >  **Admin Exchange**.</span><span class="sxs-lookup"><span data-stu-id="38eb8-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="38eb8-104">Accesați **organization**  >  **partajarea organizației**.</span><span class="sxs-lookup"><span data-stu-id="38eb8-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="38eb8-105">Sub **Partajare organizație**, faceți clic pe **Nou** .</span><span class="sxs-lookup"><span data-stu-id="38eb8-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="38eb8-106">În **noua relație de organizare**, în caseta Nume **relație,** tastați un nume prietenos pentru relația de organizație.</span><span class="sxs-lookup"><span data-stu-id="38eb8-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="38eb8-107">În caseta **Domenii de partajat cu,** tastați domeniul pentru organizația locală Externă Office 365 sau Exchange pe care doriți să o permiteți să vedeți calendarele.</span><span class="sxs-lookup"><span data-stu-id="38eb8-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="38eb8-108">Dacă trebuie să introduceți mai multe domenii, separați numele de domenii cu o virgulă.</span><span class="sxs-lookup"><span data-stu-id="38eb8-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="38eb8-109">De exemplu, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="38eb8-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="38eb8-110">Bifați caseta de selectare **Activare partajare informații liber/ocupat calendar** pentru a activa partajarea calendarului cu domeniile pe care le-ați listat.</span><span class="sxs-lookup"><span data-stu-id="38eb8-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="38eb8-111">Setați nivelul de partajare pentru informațiile din calendar liber/ocupat și setați utilizatorii care pot partaja informațiile de calendar liber/ocupat.</span><span class="sxs-lookup"><span data-stu-id="38eb8-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="38eb8-112">Pentru a seta nivelul de acces liber/ocupat, selectați una dintre următoarele:</span><span class="sxs-lookup"><span data-stu-id="38eb8-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="38eb8-113">**Informații despre calendar liber/ocupat numai cu timp**</span><span class="sxs-lookup"><span data-stu-id="38eb8-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="38eb8-114">**Calendar liber/ocupat cu timpul, subiectul și locația**</span><span class="sxs-lookup"><span data-stu-id="38eb8-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="38eb8-115">Pentru a seta utilizatorii care vor partaja informațiile din calendar liber/ocupat, selectați una dintre următoarele:</span><span class="sxs-lookup"><span data-stu-id="38eb8-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="38eb8-116">**Toate persoanele din organizația dvs.**</span><span class="sxs-lookup"><span data-stu-id="38eb8-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="38eb8-117">**Un grup de securitate specificat**</span><span class="sxs-lookup"><span data-stu-id="38eb8-117">**A specified security group**</span></span>  

<span data-ttu-id="38eb8-118">Faceți clic pe **răsfoire** pentru a alege grupul de securitate dintr-o listă, apoi faceți clic pe **ok**.</span><span class="sxs-lookup"><span data-stu-id="38eb8-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="38eb8-119">Faceți clic pe **salvare** pentru a crea relația de organizație.</span><span class="sxs-lookup"><span data-stu-id="38eb8-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="38eb8-120">**Notă:** Configurațiile între entități găzduite nu acceptă persoanele de contact personale pentru căutarea liber/ocupat.</span><span class="sxs-lookup"><span data-stu-id="38eb8-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="38eb8-121">Persoanele de contact trebuie incluse în lista globală de adrese pentru ca căutarea liber/ocupat să funcționeze.</span><span class="sxs-lookup"><span data-stu-id="38eb8-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="38eb8-122">**Pentru o înțelegere completă a acestui subiect vă rugăm să citiți:**</span><span class="sxs-lookup"><span data-stu-id="38eb8-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="38eb8-123">Crearea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="38eb8-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="38eb8-124">Modificarea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="38eb8-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="38eb8-125">Eliminarea unei relații de organizație în Exchange Online</span><span class="sxs-lookup"><span data-stu-id="38eb8-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
