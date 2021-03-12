---
title: Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708974"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="d0e98-102">Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d0e98-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="d0e98-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="d0e98-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d0e98-104">Unele mesaje de eroare comune și pașii de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="d0e98-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="d0e98-105">**PAC dispozitiv atinsă** Utilizatorul are mai multe dispozitive înscriși decât limita dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="d0e98-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d0e98-106">Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d0e98-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="d0e98-107">**Acest serviciu nu este acceptat. Nicio politică de înscriere:** serviciul de notificare Push Apple (APNs) trebuie să fie configurat sau reînnoit.</span><span class="sxs-lookup"><span data-stu-id="d0e98-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="d0e98-108">Revizuiți [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre cum să faceți acest lucru.</span><span class="sxs-lookup"><span data-stu-id="d0e98-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="d0e98-109">**Tipul de licență de utilizator nu este valid sau numele de utilizator nu este recunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="d0e98-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d0e98-110">Revizuiți aceste documente pentru a atribui o licență prin: [Centrul de administrare Office](https://docs.microsoft.com/intune/licenses-assign) sau [portalul Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="d0e98-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="d0e98-111">Resurse suplimentare pentru a vă ajuta să rezolvați problema:</span><span class="sxs-lookup"><span data-stu-id="d0e98-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d0e98-112">Utilizați [portalul de depanare Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și a rezolva erorile de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="d0e98-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d0e98-113">Revizuiți [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="d0e98-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d0e98-114">Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și [Depanare Doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d0e98-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="d0e98-115">[Aflați cum să Înscrieți dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="d0e98-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

