---
title: Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689966"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum.
  
Câteva probleme comune și pașii de rezolvare:
  
 **Eroare de dispozitiv necriptat în portalul firmei:** Versiunile mai noi de Android, mai ales începând cu v 7.0, necesită o parolă de pornire pentru a vă asigura că dispozitivul este complet criptat. Soluțiile comune sunt activarea unui cod PIN de pornire sau criptare completă a dispozitivului. Revizuiți [acest document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pentru mai multe informații.
  
 **Dispozitivele nu reușesc să facă check-in cu serviciul Intune sau să se afișeze ca "nesănătoase" în consola de administrare Intune:** Este posibil ca unele dispozitive Samsung 4,4 și 5,5 să nu se poată consulta în serviciu. Există 3 soluții posibile la această problemă:
  
1. Deschideți manual aplicația portal firmă Intune, care va iniția automat sincronizarea dispozitivelor.

2. Actualizați dispozitivul la Android 6,0 sau o versiune ulterioară.

3. Dezactivați Samsung Smart Manager din gestionarea portalului firmei Intune. Revizuiți [acest document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pentru mai multe detalii despre aceste probleme și rezoluții.

 **Tip de licență de utilizator nevalid** sau **nume utilizator nerecunoscut:** utilizatorul trebuie să i se atribuie o licență Intune sau EMS. Revizuiți aceste documente pentru a atribui o licență prin: centrul de administrare Office sau portalul Azure.
  
Resurse suplimentare pentru a vă ajuta să rezolvați problema:
  
1. Utilizați [portalul de depanare Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și a rezolva erorile de înscriere comune. Revizuiți [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

2. Revizuiți [acest document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea și rezoluțiile la fiecare.

3. [Aflați cum să Înscrieți dispozitivele Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
