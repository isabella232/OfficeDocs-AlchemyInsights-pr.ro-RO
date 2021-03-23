---
title: Notificare Dan Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037239"
---
# <a name="notification-aad-connect"></a>Notificare Dan Connect

- Asigurați-vă că sunteți autorizat să efectuați operațiunea. Administratorii globali au acces în mod implicit. În plus, puteți utiliza [controlul Access bazat pe roluri](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) pentru a delega permisiunea de înregistrare la colaborator.
- Asigurați-vă că punctele finale necesare sunt activate și nu sunt blocate din cauza firewallului. Pentru detalii, consultați [cerințe](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Înregistrarea poate să nu reușească din cauza comunicării de ieșire supusă inspecției SSL de către stratul de rețea.
- Asigurați-vă că ați verificat setările de notificare pentru Azure AD Connect Health și revizuiți setarea. Pentru a înțelege cum să configurați setările de notificare pentru notificările de sănătate Azure AD Connect, consultați acest [Ghid](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Pentru a afla mai multe despre raportul de sincronizare de la AAD Connect Health și despre cum să îl descărcați, consultați [raportul de sincronizare la nivel de obiect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Pentru a depana avertizările de sănătate din AAD Connect, urmați [Ghidul de depanare pentru depanarea alertelor de stare a stării](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) de bună funcționare a datelor și pentru întrebări frecvente, consultați [întrebări frecvente despre instalarea](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problemelor de sănătate.
