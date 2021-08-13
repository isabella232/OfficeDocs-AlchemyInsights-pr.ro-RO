---
title: Depanarea problemelor cu înscrierea Windows dispozitive în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981053"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea Windows dispozitive în Microsoft Intune

Revizuiți resursele listate mai jos pentru a rezolva problema acum.
  
Câțiva mesaje de eroare comune și pași de rezolvare:
  
 **Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dvs. de cont a expirat. Descărcați din nou pachetul de software client pentru PC din consola de administrare Intune. Consultați această documentație pentru mai multe informații.
  
 **Cod de 0x801c0003:** Eroarea poate apărea în următoarele scenarii:
  
-  Utilizatorul are mai multe dispozitive înscrise decât limita pentru dispozitive. Revizuiți aceste documente pentru [a elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau a modifica limita pentru [dispozitive.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Utilizatorii pot uni dispozitive la Azure AD" este setată la "fără". Setați-o pentru toți utilizatorii sau selectați-o. Consultați [această documentație](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informații.

-  Dispozitivul este înscris deja de alt utilizator. În acest caz, eliminați dispozitivul din consola Azure Intune sau anularea manuală a controlului dispozitivului înainte de a încerca din nou.

-  Dispozitivul este Windows 10 Home. Doar SKU Windows 10 Pro SKU-ul pentru educație și întreprinderi se pot alătura Azure Active Directory.

Resurse suplimentare care ajută la rezolvarea problemei:
  
-  Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere. Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

-  Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru [fiecare:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Ghid de depanare și [Document de depanare.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Aflați cum să vă înscrieți Windows dispozitive în Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
