---
title: Problemă cu AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483117"
---
# <a name="problem-with-aad-connect-health"></a>Problemă cu AAD Connect Health

- Asigurați-vă că sunteți autorizat să efectuați operațiunea. Administratorii globali au acces în mod implicit. În plus, puteți utiliza [controlul Access bazat pe roluri](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) pentru a delega permisiunea de înregistrare la colaborator.
- Asigurați-vă că punctele finale necesare sunt activate și nu sunt blocate din cauza firewallului. Pentru detalii, consultați [cerințe](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Înregistrarea poate să nu reușească din cauza comunicării de ieșire supusă inspecției SSL de către stratul de rețea.
- Asigurați-vă că ați verificat setările de notificare pentru Azure AD Connect Health. Vă rugăm să vă revizuiți setarea. Acest [Ghid](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vă poate ajuta să înțelegeți cum să configurați setările de notificare pentru notificările de sănătate Azure AD Connect.
- Pentru a afla mai multe despre raportul de sincronizare de la AAD Connect Health și despre cum să îl descărcați, consultați [raportul de sincronizare la nivel de obiect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Pentru a depana avertizările de sănătate din Dan Connect, urmați [Ghidul de depanare pentru depanarea alertelor de stare a stării de sănătate](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) și pentru întrebări frecvente, consultați [întrebări comune despre instalarea](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problemelor de sănătate.
