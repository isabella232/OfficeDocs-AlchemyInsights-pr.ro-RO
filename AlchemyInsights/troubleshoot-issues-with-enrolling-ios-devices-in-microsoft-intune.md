---
title: Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823475"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e2ae5-102">Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e2ae5-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e2ae5-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e2ae5-104">Câțiva mesaje de eroare comune și pași de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="e2ae5-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e2ae5-105">**S-a atins capacul dispozitivului** Utilizatorul are mai multe dispozitive înscrise decât limita pentru dispozitive.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e2ae5-106">Revizuiți aceste documente pentru [a elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau a modifica limita pentru [dispozitive.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e2ae5-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e2ae5-107">**Acest serviciu nu este acceptat. Nicio politică de înscriere:** Serviciul de notificare push (APNS) Apple trebuie să fie configurat sau reînnoit.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e2ae5-108">Consultați [acest document pentru](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) instrucțiuni despre cum să faceți acest lucru.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e2ae5-109">**Tipul de licență de utilizator este nevalid sau Nume de utilizator nerecunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e2ae5-110">Revizuiți aceste documente pentru a atribui o licență prin: [Centrul de administrare Office](https://docs.microsoft.com/intune/licenses-assign) sau portalul [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="e2ae5-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e2ae5-111">Resurse suplimentare care ajută la rezolvarea problemei:</span><span class="sxs-lookup"><span data-stu-id="e2ae5-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e2ae5-112">Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e2ae5-113">Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="e2ae5-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e2ae5-114">Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru [fiecare:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Ghid de depanare și [Document de depanare.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e2ae5-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e2ae5-115">[Aflați cum să înscrieți dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="e2ae5-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

