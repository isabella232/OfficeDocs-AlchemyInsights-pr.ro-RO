---
title: Instalarea Office pe un terminal server-fără licență
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205421"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="c4213-102">Instalarea Office pe un server terminal</span><span class="sxs-lookup"><span data-stu-id="c4213-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="c4213-103">Pentru implementarea Office 365 ProPlus pe un Windows Server utilizând consolidare servicii Desktop la distanță (RDS), denumit anterior Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="c4213-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="c4213-104">Trebuie să aveți un plan Office 365 care include Office 365 ProPlus, ar fi Office 365 Enterprise E3 sau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="c4213-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="c4213-105">Planurile Office 365 Business și Office 365 Business Premium nu includ Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="c4213-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="c4213-106">Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c4213-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="c4213-107">Dacă doriți să instalați Office 365 ProPlus pe RDS de la centrul de administrare Microsoft 365, ***care utilizează setările de instalare implicite***, utilizați pașii următori.</span><span class="sxs-lookup"><span data-stu-id="c4213-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="c4213-108">De asemenea, aveți posibilitatea să descărcați și să executați [Asistentul Microsoft pentru asistență și recuperare](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Office 365 ProPlus în modul de activare a computerului partajat.</span><span class="sxs-lookup"><span data-stu-id="c4213-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="c4213-109">Verificați ce Office 365 plan aveți.</span><span class="sxs-lookup"><span data-stu-id="c4213-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="c4213-110">Aflați</span><span class="sxs-lookup"><span data-stu-id="c4213-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="c4213-111">Dacă este necesar, comutați la un alt plan Office 365.</span><span class="sxs-lookup"><span data-stu-id="c4213-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="c4213-112">Aflați</span><span class="sxs-lookup"><span data-stu-id="c4213-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="c4213-113">Dacă Office este deja instalat pe serverul RDS utilizând orice alte planuri de Office 365, dezinstalați-l.</span><span class="sxs-lookup"><span data-stu-id="c4213-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="c4213-114">De exemplu, mergând la panoul \> de control Dezinstalați un program.</span><span class="sxs-lookup"><span data-stu-id="c4213-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="c4213-115">Dezinstalați utilizând [asistența Microsoft și asistentul de recuperare](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă executați probleme.</span><span class="sxs-lookup"><span data-stu-id="c4213-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="c4213-116">Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [Instalați Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="c4213-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="c4213-117">După ce Office este instalat, ***nu deschideți sau faceți sign in*** la orice aplicații Office.</span><span class="sxs-lookup"><span data-stu-id="c4213-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="c4213-118">Pe serverul RDS, activați activarea computerului partajat editând registry urmând acești pași:</span><span class="sxs-lookup"><span data-stu-id="c4213-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="c4213-119">Faceți clic dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați executare.</span><span class="sxs-lookup"><span data-stu-id="c4213-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="c4213-120">În caseta Deschidere, tastați **regedit**, apoi selectați OK.</span><span class="sxs-lookup"><span data-stu-id="c4213-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="c4213-121">Selectați Da când vi se solicită să permiteți Registry Editor să facă modificări pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="c4213-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="c4213-122">În editorul de registry, adăugați o valoare șir de **Sharedcomputerlicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="c4213-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="c4213-123">Pe serverul RDS, ***Conectați-vă ca utilizator final*** și [Verificați că activarea computerului partajat este activată pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="c4213-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="c4213-124">Pentru mai multe detalii despre cerințe preliminare, instrucțiuni de instalare și îndrumare pe instalări particularizate utilizând instrumentul de implementare Office, consultați [implementarea office 365 ProPlus utilizând consolidare servicii Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="c4213-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="c4213-125">Pentru a remedia erorile legate de activarea computerului partajat, consultați [Depanarea problemelor cu activarea computerului partajat pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c4213-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  