---
title: Depanarea problemelor de asociere Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939931"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Depanarea problemelor de asociere Azure AD

1. În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit Introducere în gestionarea dispozitivelor în [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) care vă va ghida despre cum să obțineți dispozitivele sub controlul Azure AD. 
1. Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, va trebui să [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) vă asigurați că ați configurat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) și că licențierea a fost configurată mai întâi.
1. Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD. Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.
1. Pentru a face implementarea uniării Azure AD, consultați [Planificarea Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Pentru mai multe detalii despre rezolvarea problemelor comune cu Azure AD Join, consultați Întrebări frecvente despre [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) și pentru Windows 10 un dispozitiv profesionist Windows 10 Pro, consultați Nu se poate alătura unui computer la Azure AD - Trebuie să faceți upgrade la [- Comunitatea Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
