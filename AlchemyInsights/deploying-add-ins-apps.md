---
title: Implementarea programelor de completare pentru Aplicații Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233546"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="00256-102">Implementarea programelor de completare pentru Aplicații Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="00256-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="00256-103">Implementarea centralizată este modul recomandat pentru implementarea Office de completare pentru utilizatori și grupuri în cadrul organizației.</span><span class="sxs-lookup"><span data-stu-id="00256-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="00256-104">Pentru a implementa programe de completare, urmați pașii de mai jos:</span><span class="sxs-lookup"><span data-stu-id="00256-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="00256-105">**Notă:** Pentru a instala programe de completare pentru Office ca utilizator individual, consultați Vizualizarea, gestionarea și instalarea programelor de [completare Office programele.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="00256-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="00256-106">De asemenea, asigurați-vă că achiziționarea individuală de Office de completare din Magazin este activată.</span><span class="sxs-lookup"><span data-stu-id="00256-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="00256-107">Pentru detalii, consultați Prevenirea descărcărilor de programe de completare prin dezactivarea descărcării Office Magazin pentru toți clienții [(cu excepția Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="00256-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="00256-108">Asigurați-vă că mediul dvs. îndeplinește cerințele pentru implementarea de programe de completare care utilizează Implementarea centralizată.</span><span class="sxs-lookup"><span data-stu-id="00256-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="00256-109">Pentru detalii, consultați [Cerințe.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="00256-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="00256-110">Accesați Pagina **Setări Aplicații**  >  **integrate**  >  **Obțineți aplicații din** centrul Microsoft 365 administrare pentru a implementa programe de completare.</span><span class="sxs-lookup"><span data-stu-id="00256-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="00256-111">Note:</span><span class="sxs-lookup"><span data-stu-id="00256-111">Notes:</span></span> 

- <span data-ttu-id="00256-112">Aplicațiile integrate necesită ca administratorul să dea permisiuni de Administrator global Exchange permisiuni de Administrator.</span><span class="sxs-lookup"><span data-stu-id="00256-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="00256-113">Atunci când implementați programe de completare pentru mai mulți utilizatori, vă recomandăm să atribuiți utilizând grupuri în loc de utilizatori individuali.</span><span class="sxs-lookup"><span data-stu-id="00256-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="00256-114">Pentru detalii, consultați [Considerații atunci când atribuiți un program de completare utilizatorilor și grupurilor.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="00256-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="00256-115">Implementarea centralizată nu acceptă utilizatorii din grupuri imbricate sau grupuri care au grupuri părinte.</span><span class="sxs-lookup"><span data-stu-id="00256-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="00256-116">Pentru detalii, consultați [Atribuirile de utilizator și de grup.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="00256-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="00256-117">Asigurați-vă că serviciul Microsoft 365 de gestionare a aplicațiilor (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') este activat pentru ca utilizatorii să se conecteze.</span><span class="sxs-lookup"><span data-stu-id="00256-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="00256-118">Pentru detalii, consultați Configurarea [proprietăților aplicațiilor.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="00256-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="00256-119">Dacă vă experimentați probleme la implementarea programelor de completare utilizând aplicații integrate, încercați să implementați [utilizând programe de completare.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="00256-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="00256-120">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="00256-120">For more information, see:</span></span>

<span data-ttu-id="00256-121">[Implementarea de programe de completare în centrul de administrare](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gestionarea programelor de completare în centrul de administrare](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizarea cmdletelor PowerShell de implementare centralizată pentru a gestiona programe de completare](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicarea Office completare utilizând Implementarea centralizată prin centrul Microsoft 365 administrare](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Depanare: Utilizatorul nu vede programele de completare](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Depanarea erorilor utilizatorilor cu Office de completare](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="00256-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>