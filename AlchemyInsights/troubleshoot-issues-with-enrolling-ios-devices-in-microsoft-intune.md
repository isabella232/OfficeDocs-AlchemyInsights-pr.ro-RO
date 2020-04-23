---
title: Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736170"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="0bf9a-102">Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0bf9a-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="0bf9a-103">Examinați resursele enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0bf9a-104">Unele mesaje de eroare comune și pași de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="0bf9a-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="0bf9a-105">**Capac dispozitiv atins** Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0bf9a-106">Examinați aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a modifica limita [dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0bf9a-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="0bf9a-107">**Acest Serviciu nu este acceptat. Nicio politică de înscriere:** Serviciul de notificare push (APNS) Apple nu trebuie configurat sau reînnoit.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="0bf9a-108">Examinați [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre se face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="0bf9a-109">**Tip de licență utilizator Nevalid sau Nume utilizator nerecunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="0bf9a-110">Examinați aceste documente pentru a atribui o licență prin: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) sau [portalazure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="0bf9a-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="0bf9a-111">Resurse suplimentare pentru a ajuta la rezolvarea problemei:</span><span class="sxs-lookup"><span data-stu-id="0bf9a-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0bf9a-112">Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0bf9a-113">Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="0bf9a-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0bf9a-114">Examinați aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvările la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și depanare [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0bf9a-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="0bf9a-115">[Aflați să înscrieți dispozitive iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="0bf9a-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

