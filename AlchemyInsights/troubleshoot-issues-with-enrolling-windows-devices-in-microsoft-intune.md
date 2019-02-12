---
title: Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934788"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune

Consultaţi resurse enumerate mai jos pentru a rezolva problema acum. 
  
Unele mesaje de eroare comune şi rezoluţie paşi:
  
 **Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dumneavoastră de cont a expirat. Re-Descarca pachetul de programe PC Client în consola de administrare Intune. Revizui această documentaţie pentru mai multe informaţii. 
  
 **Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele situaţii: 
  
1. Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv. Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Utilizatorii pot adera dispozitive azuriu AD" este setat la "niciunul". Setaţi-l la toate sau selectaţi utilizatorii. Revizui [această documentaţie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informaţii. 
    
3. Aparatul este înscris de un alt utilizator. Dacă este cazul, eliminaţi dispozitivul din consola de Azure Intune sau unenroll manual aparatul înainte de a încerca din nou.
    
4. Aparatul este Windows 10 Home. Numai Windows 10 Pro, educaţie şi Enterprise SKU se poate alătura Azure Active Directory.
    
Resurse suplimentare pentru a rezolva problema:
  
1. Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii. 
    
2. Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) şi [Depanare doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Aflaţi cum să înscrie dispozitive Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

