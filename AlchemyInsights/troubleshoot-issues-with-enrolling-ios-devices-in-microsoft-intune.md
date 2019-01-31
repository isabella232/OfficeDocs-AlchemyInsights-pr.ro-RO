---
title: Depanarea problemelor cu inscrierea dispozitivele iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658451"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="d7088-102">Depanarea problemelor cu inscrierea dispozitivele iOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d7088-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="d7088-103">Consultaţi resurse enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="d7088-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d7088-104">Unele mesaje de eroare comune şi rezoluţie paşi:</span><span class="sxs-lookup"><span data-stu-id="d7088-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="d7088-p101">**Cap de aparat ajunge** Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv. Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d7088-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="d7088-p102">**Acest serviciu nu este acceptată. Nici o politică de înscriere:** Apple Push Notification serviciu (APNS) trebuie să fie configurat sau reînnoit. Consultaţi [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucţiuni despre cum să faci asta.</span><span class="sxs-lookup"><span data-stu-id="d7088-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="d7088-p103">**User a da un permis tip incorectă sau numele de utilizator nu este recunoscut:** Utilizatorul trebuie să li se atribuie o licenţă Intune sau EMS. Examina aceste documente pentru a atribui o licenţă prin: [Centrul de administrare birou](https://docs.microsoft.com/intune/licenses-assign) sau [portal de Azur](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="d7088-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="d7088-111">Resurse suplimentare pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="d7088-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d7088-p104">Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="d7088-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d7088-114">Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) şi [Depanare doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d7088-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="d7088-115">[Aflaţi cum să înscrie dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="d7088-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

