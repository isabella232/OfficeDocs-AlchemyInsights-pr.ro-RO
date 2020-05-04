---
title: Instalarea biroului pe un Terminal Server - Fără licență
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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010626"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="701fc-102">Instalarea Office pe un Terminal Server</span><span class="sxs-lookup"><span data-stu-id="701fc-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="701fc-103">Pentru implementarea Microsoft 365 Apps for enterprise pe un Windows Server utilizând Remote Desktop Services (RDS), denumit anterior Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="701fc-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="701fc-104">Trebuie să aveți un abonament Microsoft 365 care include Microsoft 365 Apps for enterprise, ar fi Office 365 Enterprise E3 sau Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="701fc-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="701fc-105">Planurile Microsoft 365 Apps for business și Microsoft 365 Apps for business Premium nu includ Microsoft 365 Apps for enterprise.</span><span class="sxs-lookup"><span data-stu-id="701fc-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="701fc-106">Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="701fc-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="701fc-107">Dacă doriți să instalați Microsoft 365 Apps for enterprise pe RDS din centrul de administrare Microsoft 365, ***care utilizează setările implicite de instalare,*** utilizați următorii pași.</span><span class="sxs-lookup"><span data-stu-id="701fc-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="701fc-108">De asemenea, puteți descărca și executa [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Microsoft 365 Apps for enterprise în modul de activare a computerului partajat.</span><span class="sxs-lookup"><span data-stu-id="701fc-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="701fc-109">Verificați ce abonament Microsoft 365 aveți.</span><span class="sxs-lookup"><span data-stu-id="701fc-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="701fc-110">Aflați</span><span class="sxs-lookup"><span data-stu-id="701fc-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="701fc-111">Dacă este necesar, comutați la un alt abonament Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="701fc-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="701fc-112">Aflați</span><span class="sxs-lookup"><span data-stu-id="701fc-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="701fc-113">Dacă Office este deja instalat pe serverul RDS utilizând orice alte abonamente Microsoft 365, dezinstalați-l.</span><span class="sxs-lookup"><span data-stu-id="701fc-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="701fc-114">De exemplu, accesăm \> Control Panel Uninstall a program.</span><span class="sxs-lookup"><span data-stu-id="701fc-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="701fc-115">Dezinstalați utilizând [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă aveți probleme.</span><span class="sxs-lookup"><span data-stu-id="701fc-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="701fc-116">Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [instalați Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="701fc-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="701fc-117">După instalarea Office, ***nu deschideți sau conectați-vă*** la nicio aplicații Office.</span><span class="sxs-lookup"><span data-stu-id="701fc-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="701fc-118">Pe serverul RDS, activați activarea computerului partajat prin editarea registry urmând acești pași:</span><span class="sxs-lookup"><span data-stu-id="701fc-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="701fc-119">Faceți clic cu butonul din dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați Executare.</span><span class="sxs-lookup"><span data-stu-id="701fc-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="701fc-120">În caseta Deschidere, tastați **regedit**, apoi selectați OK.</span><span class="sxs-lookup"><span data-stu-id="701fc-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="701fc-121">Selectați Da atunci când vi se solicită să permiteți Registry Editor să efectueze modificări pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="701fc-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="701fc-122">În Registry Editor, adăugați o valoare șir de **SharedComputerLicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="701fc-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="701fc-123">Pe serverul RDS, ***conectați-vă ca utilizator final*** și [verificați dacă activarea computerului partajat este activată pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="701fc-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="701fc-124">Pentru mai multe detalii despre cerințele preliminare, instrucțiunile de instalare și instrucțiuni privind instalările particularizate utilizând Instrumentul de implementare Office, consultați [Implementarea aplicațiilor Microsoft 365 pentru întreprinderi utilizând Serviciile Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="701fc-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="701fc-125">Pentru a remedia erorile legate de activarea computerului partajat, consultați [Depanarea problemelor cu activarea computerului partajat pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="701fc-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  