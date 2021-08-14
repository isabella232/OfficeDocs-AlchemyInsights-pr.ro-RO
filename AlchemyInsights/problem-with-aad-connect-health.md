---
title: Problemă cu starea Conectare AAD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923764"
---
# <a name="problem-with-aad-connect-health"></a>Problemă cu starea Conectare AAD

- Asigurați-vă că sunteți autorizat să efectuați operațiunea. Administratorii globali au acces în mod implicit. În plus, puteți utiliza Controlul accesului [pe bază de rol pentru](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) a delega permisiunea de înregistrare la Colaborator.
- Asigurați-vă că punctele finale necesare sunt activate, nu blocate din cauza firewallului. Pentru detalii, consultați [cerințele](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Înregistrarea poate să nu reușească din cauza comunicațiilor de ieșire care sunt supuse inspectării SSL la nivel de rețea.
- Asigurați-vă că ați verificat setările de notificare pentru Azure AD Conectare Health. Revizuiți setarea. Acest [ghid vă](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) poate ajuta să înțelegeți cum să configurați setările de notificare pentru Azure AD Conectare de sănătate.
- Pentru a afla mai multe despre AAD și Conectare sincronizare stare și cum să-l descărcați, consultați Raportul de sincronizare [la nivel de obiect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Pentru a depana avertizările AAD Conectare Pentru mai multe informații despre sănătate, urmați Ghidul de depanare pentru avertizările privind starea de sănătate din [AAD Conectare](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Și pentru întrebări frecvente, consultați Întrebări comune despre instalarea datelor pentru [AAD Conectare](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)Health .
