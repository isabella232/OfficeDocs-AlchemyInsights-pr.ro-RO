---
title: Depanarea asocierii la Azure AD hibrid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401919"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Depanarea asocierii la Azure AD hibrid

Se recomandă ferm să vă asigurați că un dispozitiv poate accesa puncte finale de înregistrare a dispozitivelor din contul de sistem, utilizând [scriptul de testare a conectivității pentru înregistrarea dispozitivelor](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că revizuiți această[introducere în gestionarea dispozitivelor în Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) pentru a afla cum să controlați dispozitivele cu Azure AD.
1. Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, asigurați-vă că ați [configurat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) și că aveți [licențierea](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) în locație mai întâi.
1. Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD și AD local. Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor. În plus, în cazul în care configurați înregistrările automate în Active Directory local, va trebui să fiți administrator Active Directory și AD FS (dacă este cazul).

Pentru mai multe detalii despre rezolvarea potențialelor probleme cu asocierea hibridă, consultați [Depanarea asocierii hibride](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) pentru configurarea Azure AD asociat și pentru gestionarea dispozitivelor utilizând portalul Azure AD, consultați [Configurarea dispozitivelor Azure AD asociate (asociate cu domenii, local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) și [Gestionarea dispozitivelor utilizând portalul Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Pentru a rezolva problemele comune cu asocierea la Azure Active Directory (AD) hibrid, consultați [Întrebări frecvente despre asocierea la Azure AD hibrid](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
