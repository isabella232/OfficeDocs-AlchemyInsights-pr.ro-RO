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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669260"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare comune și pașii de rezolvare:
  
- **PAC dispozitiv atinsă** Utilizatorul are mai multe dispozitive înscriși decât limita dispozitivului. Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Acest serviciu nu este acceptat. Nicio politică de înscriere:** serviciul de notificare Push Apple (APNs) trebuie să fie configurat sau reînnoit. Revizuiți [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre cum să faceți acest lucru. 
    
- **Tipul de licență de utilizator nu este valid sau numele de utilizator nu este recunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS. Revizuiți aceste documente pentru a atribui o licență prin: [Centrul de administrare Office](https://docs.microsoft.com/intune/licenses-assign) sau [portalul Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Resurse suplimentare pentru a vă ajuta să rezolvați problema:
  
1. Utilizați [portalul de depanare Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și a rezolva erorile de înscriere comune. Revizuiți [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii. 
    
2. Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și [Depanare Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Aflați cum să Înscrieți dispozitivele iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

