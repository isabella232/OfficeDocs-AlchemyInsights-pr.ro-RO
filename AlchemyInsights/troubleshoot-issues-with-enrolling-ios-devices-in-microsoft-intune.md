---
title: Depanarea problemelor cu inscrierea dispozitivele iOS în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391019"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Depanarea problemelor cu inscrierea dispozitivele iOS în Microsoft Intune

Consultaţi resurse enumerate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare comune şi rezoluţie paşi:
  
- **Cap de aparat ajunge** Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv. Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Acest serviciu nu este acceptată. Nici o politică de înscriere:** Apple Push Notification serviciu (APNS) trebuie să fie configurat sau reînnoit. Consultaţi [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucţiuni despre cum să faci asta. 
    
- **User a da un permis tip incorectă sau numele de utilizator nu este recunoscut:** Utilizatorul trebuie să li se atribuie o licenţă Intune sau EMS. Examina aceste documente pentru a atribui o licenţă prin: [Centrul de administrare birou](https://docs.microsoft.com/intune/licenses-assign) sau [portal de Azur](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Resurse suplimentare pentru a rezolva problema:
  
1. Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii. 
    
2. Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) şi [Depanare doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Aflaţi cum să înscrie dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

