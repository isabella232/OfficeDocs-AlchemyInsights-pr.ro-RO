---
title: Depanarea problemelor cu înscrierea dispozitive iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507015"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="21b1c-102">Depanarea problemelor cu înscrierea dispozitive iOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="21b1c-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="21b1c-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="21b1c-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="21b1c-104">Unele mesaje de eroare obișnuite și pașii de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="21b1c-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="21b1c-105">**Capac dispozitiv atins** Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="21b1c-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="21b1c-106">Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="21b1c-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="21b1c-107">**Acest serviciu nu este acceptat. Nicio politică de înscriere:** serviciul de notificare Push Apple (APNS) trebuie să fie configurat sau reînnoit.</span><span class="sxs-lookup"><span data-stu-id="21b1c-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="21b1c-108">Examinați [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre se face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="21b1c-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="21b1c-109">**Tip licență utilizator invalid sau nume utilizator nerecunoscut:** Utilizatorul trebuie să i se atribuie o licență Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="21b1c-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="21b1c-110">Examinați aceste documente pentru a atribui o licență prin: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) sau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="21b1c-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="21b1c-111">Resurse suplimentare pentru a vă rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="21b1c-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="21b1c-112">Utilizați [Intune depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva eșecuri de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="21b1c-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="21b1c-113">Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="21b1c-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="21b1c-114">Revizuiți aceste documente pentru o listă de erori obișnuite care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și [Depanare Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="21b1c-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="21b1c-115">[Aflați să înregistrați dispozitive iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="21b1c-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

