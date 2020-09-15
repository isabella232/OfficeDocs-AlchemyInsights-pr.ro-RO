---
title: Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658890"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum.
  
Unele mesaje de eroare comune și pașii de rezolvare:
  
 **Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul de cont a expirat. Descărcați din nou pachetul software client PC în consola de administrare Intune. Revizuiți această documentație pentru mai multe informații.
  
 **Codul de eroare 0x801c0003:** Eroarea poate apărea în următoarele scenarii:
  
-  Utilizatorul are mai multe dispozitive înscriși decât limita dispozitivului. Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Utilizatorii se pot asocia dispozitivelor la Azure AD" este setat la "None". Setați-o la toate sau selectați utilizatori. Revizuiți [această documentație](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informații.

-  Dispozitivul este deja înscris de alt utilizator. Dacă acesta este cazul, eliminați dispozitivul din consola Azure Intune sau deînscrie manual dispozitivul înainte de a încerca din nou.

-  Dispozitivul este Windows 10 Home. Doar Windows 10 Pro, Education și SKU-ul Enterprise se pot asocia la Azure Active Directory.

Resurse suplimentare pentru a vă ajuta să rezolvați problema:
  
-  Utilizați [portalul de depanare Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și a rezolva erorile de înscriere comune. Revizuiți [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

-  Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) și [Depanare Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Aflați cum să Înscrieți dispozitivele Windows în Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
