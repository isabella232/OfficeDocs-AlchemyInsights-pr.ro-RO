---
title: Depanarea problemelor cu inscrierea dispozitive Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485188"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6d817-102">Depanarea problemelor cu inscrierea dispozitive Android în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6d817-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6d817-103">Consultaţi resurse enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="6d817-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6d817-104">Unele probleme comune şi rezoluţie paşi:</span><span class="sxs-lookup"><span data-stu-id="6d817-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6d817-p101">**Aparat nu criptate eroare în compania Portal:** Versiunile mai noi de Android, în special începând cu v7.0, cere o parola de startup pentru a vă asigura că dispozitivul este complet criptat. Soluţiile comune sunt pentru a activa un cod pin startup sau cripta complet dispozitivul. Revizuirea [acestui document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="6d817-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="6d817-p102">**Dispozitive nu verifica cu serviciul Intune sau afişa ca "Nesanatoase" în consola de administrare Intune:** Unele 4.4 Samsung şi 5,5 dispozitive pot verifica în service. Există 3 posibile soluţii la această problemă:</span><span class="sxs-lookup"><span data-stu-id="6d817-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="6d817-110">Manual deschide aplicaţia Portal de compania Intune, care va iniţia automat o sincronizare dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="6d817-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="6d817-111">Actualizați dispozitivul Android 6.0 sau mai mare.</span><span class="sxs-lookup"><span data-stu-id="6d817-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="6d817-p103">Dezactivaţi Samsung Smart Manager la gestionarea Intune compania Portal. Revizuirea [acestui document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , pentru mai multe detalii despre aceste probleme şi rezoluţii.</span><span class="sxs-lookup"><span data-stu-id="6d817-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="6d817-p104">**User a da un permis tip nevalid** sau **User nume nu a fost recunoscut eroarea:** utilizatorul trebuie să li se atribuie o licenţă Intune sau EMS. Examina aceste documente pentru a atribui o licenţă prin: centrul de administrare Office sau Azure portal.</span><span class="sxs-lookup"><span data-stu-id="6d817-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="6d817-116">Resurse suplimentare pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="6d817-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6d817-p105">Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/en-us/intune/help-desk-operators) , pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="6d817-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="6d817-119">Consultaţi [acest document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare.</span><span class="sxs-lookup"><span data-stu-id="6d817-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="6d817-120">[Aflaţi cum să înscrie dispozitive Android în Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="6d817-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

