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
    

