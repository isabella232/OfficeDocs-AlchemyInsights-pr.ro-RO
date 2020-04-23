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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor iOS în Microsoft Intune

Examinați resursele enumerate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare comune și pași de rezolvare:
  
- **Capac dispozitiv atins** Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv. Examinați aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a modifica limita [dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Acest Serviciu nu este acceptat. Nicio politică de înscriere:** Serviciul de notificare push (APNS) Apple nu trebuie configurat sau reînnoit. Examinați [acest document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pentru instrucțiuni despre se face acest lucru. 
    
- **Tip de licență utilizator Nevalid sau Nume utilizator nerecunoscut:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS. Examinați aceste documente pentru a atribui o licență prin: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) sau [portalazure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Resurse suplimentare pentru a ajuta la rezolvarea problemei:
  
1. Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune. Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii. 
    
2. Examinați aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvările la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și depanare [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Aflați să înscrieți dispozitive iOS în Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

