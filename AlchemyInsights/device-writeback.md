---
title: Writeback dispozitivului
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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256859"
---
# <a name="device-writeback"></a>Writeback dispozitivului

Writeback dispozitivului este utilizat în următoarele scenarii:

- Activarea [Windows Hello pentru Business utilizând implementarea certificatelor hibride de încredere](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Activarea accesului condiționat pe baza dispozitivelor la aplicații protejate ADFS (2012 R2 sau mai mare) (bazându-se pe trusturi de partid)

    > [!NOTE]
    > Un abonament la Azure AD Premium este necesar pentru device writeback.

Aceasta oferă securitate suplimentară și asigurare că accesul la aplicații se acordă doar dispozitivelor de încredere. Pentru mai multe informații despre accesul condiționat, consultați [gestionarea riscului cu acces condiționat](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) și [Configurarea accesului condiționat local utilizând înregistrarea dispozitivelor Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).

Pentru mai multe informații despre activarea dispozitivelor writeback pentru dispozitive, consultați [Activarea dispozitivelor writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
