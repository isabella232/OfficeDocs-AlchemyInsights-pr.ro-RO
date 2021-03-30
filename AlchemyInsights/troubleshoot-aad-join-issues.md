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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405758"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Depanarea problemelor de asociere Azure AD

1. În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit Introducere în gestionarea dispozitivelor în [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) care vă va ghida cum să duceți dispozitivele sub controlul Azure AD. 
1. Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, va trebui să [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) vă asigurați că ați configurat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) și că licențierea a fost configurată mai întâi.
1. Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD. Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.
1. Pentru a face implementarea uniării Azure AD, consultați [Planificarea Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Pentru mai multe detalii despre rezolvarea problemelor comune cu Azure AD join consultați Întrebări frecvente despre [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) și pentru dispozitivul Windows 10 pro, consultați Nu se poate alătura computerului [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) la Azure AD - Trebuie să faceți upgrade la - Comunitatea Microsoft
