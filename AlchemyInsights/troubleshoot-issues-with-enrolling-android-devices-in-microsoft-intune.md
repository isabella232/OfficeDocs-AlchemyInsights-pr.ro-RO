---
title: Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008090"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum.
  
Câțiva pași uzuali pentru probleme și rezolvare:
  
 **Eroarea Dispozitiv fără criptare în Portal firmă:** Versiunile mai noi de Android, în special începând cu v7.0, necesită un cod de acces la pornire pentru a vă asigura că dispozitivul dvs. este complet criptat. Soluțiile obișnuite sunt cele de a activa un cod PIN de pornire sau a cripta complet dispozitivul. Consultați [acest document pentru](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) mai multe informații.
  
 **Dispozitivele nu reușesc să se verifice cu serviciul Intune sau să se afișeze ca "Nesăcoase" în consola de administrare Intune:** Este posibil ca unele dispozitive Samsung 4.4 și 5.5 să nu intre în serviciu. Există 3 soluții posibile pentru această problemă:
  
1. Deschideți manual aplicația Portal firmă Intune, care va iniția automat o sincronizare a dispozitivului.

2. Actualizați dispozitivul la Android 6.0 sau o versiune mai recentă.

3. Dezactivați Samsung Smart Manager pentru a gestiona Portal firmă Intune. Consultați [acest document pentru](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) detalii suplimentare despre aceste probleme și rezolvări.

 **Tipul de licență de utilizator** Eroare nevalidă sau Nume de utilizator nerecunoscut: Utilizatorului trebuie să i se atribuie o licență Intune sau EMS.  Revizuiți aceste documente pentru a atribui o licență prin: Office de administrare sau portalul Azure.
  
Resurse suplimentare care ajută la rezolvarea problemei:
  
1. Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere. Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

2. Revizuiți [acest document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru fiecare.

3. [Aflați cum să înscrieți dispozitive Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
