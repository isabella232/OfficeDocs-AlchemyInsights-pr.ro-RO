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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitive iOS în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare obișnuite și pașii de rezolvare:
  
- **Capac dispozitiv atins** Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv. Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Acest serviciu nu este acceptat. Nicio politică de înscriere:** serviciul de notificare Push Apple (APNS) trebuie să fie configurat sau reînnoit. Examinați [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre se face acest lucru. 
    
- **Tip licență utilizator invalid sau nume utilizator nerecunoscut:** Utilizatorul trebuie să i se atribuie o licență Intune sau EMS. Examinați aceste documente pentru a atribui o licență prin: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) sau [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Resurse suplimentare pentru a vă rezolva problema:
  
1. Utilizați [Intune depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva eșecuri de înscriere comune. Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii. 
    
2. Revizuiți aceste documente pentru o listă de erori obișnuite care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și [Depanare Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Aflați să înregistrați dispozitive iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

