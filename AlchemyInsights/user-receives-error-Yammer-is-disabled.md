---
title: Utilizatorul primește eroarea AADSTS7000112 Yammer este dezactivat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198374"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Utilizatorul primește eroarea AADSTS7000112 Yammer este dezactivat

Dacă primiți eroarea "AADSTS7000112: Aplicația '00000005-0000-0ff1-ce00-00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 Este posibil ca un administrator să fi dezactivat principalul serviciului pentru a bloca accesul la Yammer.

Dezactivarea principalului serviciului nu este recomandată și poate provoca probleme suplimentare. Pentru mai multe informații despre abordarea acceptată pentru a bloca accesul utilizatorilor la Yammer, consultați [Dezactivarea accesului Yammer pentru utilizatorii Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Pentru a corecta această problemă în portalul Azure și a restabili accesul utilizatorului la Yammer:

1.  Deschideți pagina Azure Active Directory și selectați **Aplicații enterprise** sub **Gestionare** în panoul de navigare din stânga.
3.  Tastați **Office 365 Yammer** în caseta de căutare și selectați numele aplicației pentru a deschide setările.
4.  Selectați **Proprietăți** sub **Gestionare** în panoul de navigare din stânga.
5.  Setați valoarea **Activat pentru ca utilizatorii să se conecteze?** **Yes** **Save**
6.  Conectați-vă din nou la Yammer. S-ar putea să trebuiți să ștergeți cookie-urile.

Alternativ, executați comenziLe PowerShell pentru a seta valoarea. Pentru mai multe informații, consultați [eroarea "Ne pare rău, dar întâmpinam probleme la conectare" atunci când faceți clic pe dala Yammer din Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 