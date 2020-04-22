---
title: Depanarea problemelor legate de înscrierea dispozitivelor Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759632"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Depanarea problemelor legate de înscrierea dispozitivelor Android în Microsoft Intune

Examinați resursele enumerate mai jos pentru a rezolva problema acum.
  
Unele probleme comune și etape de rezolvare:
  
 **Dispozitiv nu criptate eroare în companie Portal:** Versiunile mai noi de Android, în special începând cu v7.0, necesită un cod de acces la pornire pentru a vă asigura că dispozitivul este complet criptat. Soluțiile comune sunt pentru a activa un pin de pornire sau pentru a cripta complet dispozitivul. Examinați [acest document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pentru mai multe informații.
  
 **Dispozitivele nu reușesc să se consulte cu serviciul Intune sau afișați ca "Nesănătoase" în consola de administrare Intune:** Este posibil ca unele dispozitive Samsung 4.4 și 5.5 să nu se verifice în serviciu. Există 3 soluții posibile la această problemă:
  
1. Deschideți manual aplicația Intune Company Portal, care va iniția automat o sincronizare a dispozitivului.

2. Actualizați dispozitivul la Android 6.0 sau mai recent.

3. Dezactivați Samsung Smart Manager de la gestionarea Portalului companiei Intune. Revizuiți [acest document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pentru detalii suplimentare cu privire la aceste probleme și rezolvări.

 **Tip de licență utilizator Invalid** sau **Nume utilizator Nerecunoscut eroare:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS. Examinați aceste documente pentru a atribui o licență prin: Office Admin Center sau portalazure.
  
Resurse suplimentare pentru a ajuta la rezolvarea problemei:
  
1. Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune. Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

2. Examinați [acest document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea și rezolvările pentru fiecare.

3. [Aflați să înscrieți dispozitive Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
