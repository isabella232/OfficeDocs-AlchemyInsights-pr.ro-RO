---
title: Permiteți unui utilizator să sincronizeze un cont personal cu contul de la locul de muncă Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813404"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permiteți unui utilizator să sincronizeze un cont personal cu contul de la locul de muncă Microsoft Edge

Asigurați-vă că îndepliniți aceste criterii:

- Enterprise State Roaming este activat în centrul de administrare Azure Active Directory, care necesită un abonament la Azure Active Directory Premium sau Enterprise Mobility + Security (EMS). Pentru mai multe informații, consultați [Activarea Enterprise State Roaming în Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Sunt îndeplinite unul sau ambele criterii următoare:
    - Serviciul Azure Information Protection este activat pentru entitatea dvs. găzduită. Pentru detalii, consultați [Activarea Protecției Azure Rights Management din Centru de administrare Microsoft 365](/azure/information-protection/activate-office365).
    - Caracteristica Azure Active Directory Enterprise State Roaming (ESR) este activată pentru orice utilizator sau entitate găzduită. Pentru mai multe informații, consultați [Ce este roamingul pentru starea de întreprindere?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Dacă AIP și ESR sunt dezactivate, un mesaj de eroare îi informează pe utilizatori că sincronizarea nu este disponibilă pentru conturile lor.
