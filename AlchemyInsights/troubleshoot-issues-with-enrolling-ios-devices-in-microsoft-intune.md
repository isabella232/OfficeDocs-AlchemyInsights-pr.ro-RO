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
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047988"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum. 
  
Câțiva mesaje de eroare comune și pași de rezolvare:
  
- **S-a atins capacul dispozitivului** Utilizatorul are mai multe dispozitive înscrise decât limita pentru dispozitive. Revizuiți aceste documente pentru [a elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau a modifica limita pentru [dispozitive.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Acest serviciu nu este acceptat. Nicio politică de înscriere:** Serviciul de notificare push (APNS) Apple trebuie să fie configurat sau reînnoit. Consultați [acest document pentru](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) instrucțiuni despre cum să faceți acest lucru. 
    
- **Tipul de licență de utilizator este nevalid sau Nume de utilizator nerecunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS. Revizuiți aceste documente pentru a atribui o licență prin: [Office de administrare](https://docs.microsoft.com/intune/licenses-assign) sau portalul [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Resurse suplimentare care ajută la rezolvarea problemei:
  
1. Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere. Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii. 
    
2. Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru [fiecare:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Ghid de depanare și [Document de depanare.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Aflați cum să înscrieți dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

