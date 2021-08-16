---
title: Writeback dispozitiv
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101962"
---
# <a name="device-writeback"></a>Writeback dispozitiv

Dispozitivul WriteBack este utilizat în următoarele scenarii:

- Activarea [Windows Hello pentru business utilizând implementarea hibridă de încredere a certificatelor](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Activarea accesului condiționat bazat pe dispozitive în aplicații protejate cu ADFS (2012 R2 sau mai mare) (încredere în partea de bază)

    > [!NOTE]
    > Este necesar un abonament la Azure AD Premium pentru writebackul dispozitivului.

Acest lucru oferă securitate și asigurări suplimentare că accesul la aplicații este acordat numai dispozitivelor de încredere. Pentru mai multe informații [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) despre accesul condiționat, consultați Gestionarea riscurilor cu accesul condiționat și Configurarea accesului condiționat local [utilizând înregistrarea Azure Active Directory dispozitive.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Pentru mai multe informații despre Activarea Writeback al dispozitivelor pentru dispozitive, consultați [Activarea WriteBack pentru dispozitive.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
