---
title: Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665844"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune

Examinați resursele enumerate mai jos pentru a rezolva problema acum.
  
Unele mesaje de eroare comune și pași de rezolvare:
  
 **Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul de cont a expirat. Descărcați din nou pachetul software PC Client în Consola de administrare Intune. Examinați această documentație pentru mai multe informații.
  
 **Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele scenarii:
  
-  Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv. Examinați aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a modifica limita [dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Utilizatorii se pot alătura dispozitivelor azure AD" este setată la "nici unul.". Setați-l la toți utilizatorii sau selectați-l. Examinați [această documentație](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informații.

-  Dispozitivul este deja înscris de un alt utilizator. Dacă acesta este cazul, eliminați dispozitivul din consola Azure Intune sau dezînscrieți manual dispozitivul înainte de a încerca din nou.

-  Dispozitivul este Windows 10 Home. Numai SKU-uri Windows 10 Pro, Educație și Întreprindere se pot alătura Azure Active Directory.

Resurse suplimentare pentru a ajuta la rezolvarea problemei:
  
-  Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune. Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.

-  Examinați aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvările la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) și depanare [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Aflați să înscrieți dispozitive Windows în Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
