---
title: Instalarea office pe un Server Terminal - fără licenţă
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918991"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b14e2-102">Instalarea Office pe un Server Terminal</span><span class="sxs-lookup"><span data-stu-id="b14e2-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b14e2-103">Pentru implementarea Office 365 ProPlus pe un Windows Server folosind Remote Desktop servicii (RDS), fostă numit Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="b14e2-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b14e2-p101">Trebuie să aveţi un plan de Office 365 care include Office 365 ProPlus, cum ar fi Office 365 Intreprindere E3 sau Intreprindere E5. Planuri Office 365 Business si Office 365 Business Premium nu includ Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="b14e2-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="b14e2-106">Aveţi nevoie pentru a permite [Activarea shared calculator](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b14e2-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="b14e2-107">Dacă doriţi să instalaţi Office 365 ProPlus pe RDS la portalul Office 365 \*\* *care utilizează setările implicite ale instalării* \*\*, urmaţi aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="b14e2-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="b14e2-p102">Verifica ce plan de Office 365 care aveţi. [Aflaţi cum](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="b14e2-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="b14e2-p103">Dacă este necesar, trecerea la o diferite Office 365 planul. [Aflaţi cum](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="b14e2-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="b14e2-p104">În cazul în care biroul este deja instalat pe serverul RDS folosind orice alte planuri Office 365, dezinstalaţi-l. De exemplu, de a merge la panoul de Control \> dezinstala un program. Uninstall folosire [Microsoft Support si asistent de recuperare](https://aka.ms/SARA-OfficeUninstall-Alchemy) în cazul în care se execută în probleme.</span><span class="sxs-lookup"><span data-stu-id="b14e2-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="b14e2-115">Pe serverul RDS, faceţi sign in la portalul Office 365 cu contul de administrator şi [instala Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b14e2-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="b14e2-116">După ce este instalat Office, \*\* *nu deschide sau conectaţi-vă* \*\* pentru orice aplicatii de birou.</span><span class="sxs-lookup"><span data-stu-id="b14e2-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="b14e2-117">Pe serverul RDS, permite activarea computer partajat prin editarea registry urmând aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="b14e2-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="b14e2-p105">Faceţi clic dreapta pe butonul de Windows în colţul din stânga jos a ecranului, şi selectaţi Executare. În Deschidere cutie, tip **regedit**, şi apoi selectaţi OK.</span><span class="sxs-lookup"><span data-stu-id="b14e2-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="b14e2-120">Selectați Da când vi se solicită să permită Registry Editor pentru a face modificări la aparatul dvs.</span><span class="sxs-lookup"><span data-stu-id="b14e2-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="b14e2-121">În Registry Editor, adăugaţi o valoare şir de **SharedComputerLicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="b14e2-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="b14e2-122">Pe serverul RDS, \*\* *conectaţi-vă ca un utilizator final* \*\* şi [să verifice că shared calculator activation is enabled pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b14e2-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="b14e2-123">Pentru mai multe detalii pe premise, instrucţiuni de configurare şi îndrumări cu privire la instalări particularizate utilizând instrumentul de implementare Office, vă rugăm să consultaţi [Implementaţi Office 365 ProPlus folosind Remote Desktop servicii](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b14e2-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="b14e2-124">Pentru a rezolva erorile legate de shared calculator activare, vă rugăm să consultaţi [Depanarea problemelor cu activare shared calculator pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="b14e2-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

