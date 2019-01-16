---
title: Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307533"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune

Consultaţi resurse enumerate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare comune şi rezoluţie paşi:
  
 **Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dumneavoastră de cont a expirat. Re-Descarca pachetul de programe PC Client în consola de administrare Intune. Revizui această documentaţie pentru mai multe informaţii. 
  
 **Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele situaţii: 
  
1. Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv. Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/en-us/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Utilizatorii pot adera dispozitive azuriu AD" este setat la "niciunul". Setaţi-l la toate sau selectaţi utilizatorii. Revizui [această documentaţie](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informaţii. 
    
3. Aparatul este înscris de un alt utilizator. Dacă este cazul, eliminaţi dispozitivul din consola de Azure Intune sau unenroll manual aparatul înainte de a încerca din nou.
    
4. Aparatul este Windows 10 Home. Numai Windows 10 Pro, educaţie şi Enterprise SKU se poate alătura Azure Active Directory.
    
Resurse suplimentare pentru a rezolva problema:
  
1. Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/en-us/intune/help-desk-operators) , pentru mai multe detalii. 
    
2. Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) şi [Depanare doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Aflaţi cum să înscrie dispozitive Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

