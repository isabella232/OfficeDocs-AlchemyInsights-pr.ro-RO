---
title: Atribuirea unui rol de jurnal de audit în centrul de conformitate & securitate Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749520"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Atribuirea unui rol de jurnal de audit în centrul de conformitate & securitate Office 365

Pentru a căuta în Jurnalul de auditare Office 365, unui administrator trebuie să i se atribuie rolul de **jurnal de audit doar pentru vizualizare** sau rolul **jurnalelor de auditare** în Exchange Online. Aceste roluri sunt atribuite în mod implicit grupurilor de roluri pentru gestionarea conformității și gestionarea organizației. Administratorii globali din Office 365 și Microsoft 365 sunt adăugați automat ca membri ai grupului de roluri Gestionare organizație.

Pentru a permite unui utilizator să caute cu nivelul minim de privilegii, creați un grup de roluri particularizat în Exchange Online, **Adăugați rolul de** jurnal de auditare pentru rolurile de **Audit doar pentru vizualizare** , apoi adăugați utilizatorul ca membru al grupului de roluri nou.

Pentru mai multe informații, consultați [gestionarea grupurilor de roluri în Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) și [căutarea în Jurnalul de auditare din centrul de conformitate & de securitate](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).