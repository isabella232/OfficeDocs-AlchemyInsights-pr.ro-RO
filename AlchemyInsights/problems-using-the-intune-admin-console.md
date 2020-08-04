---
title: Probleme la utilizarea consolei de administrare Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555390"
---
# <a name="problems-using-the-intune-admin-console"></a>Probleme la utilizarea consolei de administrare Intune

**"Acces refuzat" atunci când navigați pe portalul de administrare Intune.**

- Dacă sunteți membru al unui rol particularizat Intune, asigurați-vă că contul dvs.
- Dacă utilizați Configuration Manager pentru a gestiona dispozitive, verificați dacă nu faceți parte din colecția de utilizatori Intune pentru Configuration Manager MDM.
- Verificați dacă vi s-au atribuit permisiunile corespunzătoare de control de administrare bazat pe roluri (RBAC) în lama rolurilor Intune.
- Verificați dacă grupul utilizat nu este o listă de distribuire. Intune din portalul Azure acceptă numai conturile de utilizator care aparțin grupurilor de securitate Azure Active Directory. Examinați grupurile în portalul Azure > **Intune**  >  **Groups**sau în Azure portal > **Azure Active Directory**.

**Utilizatorul are prea multe permisiuni pentru rolul Intune atribuit**

Sfătuiți utilizatorul să meargă la **Intune**  >  **Intune roluri**  >  **Permisiunile mele**  >  **Export** pentru a revizui permisiunile acordate.

**Am adăugat un grup de domenii la un rol, dar utilizatorii din acel rol văd în continuare alți utilizatori sau dispozitive.**

Grupurile de domenii nu filtrează utilizatorii sau dispozitivele. Grupuri de domenii:

- Limitați utilizatorii cărora le pot atribui politici sau aplicații.
- Se permite numai anumitor utilizatori să execute activități la distanță pe dispozitive.

Pentru mai multe informații despre grupurile de domenii, consultați [Controlul accesului bazat pe roluri (RBAC) cu Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Am adăugat un utilizator la un rol Intune, dar ei încă mai au acces deplin la consola de admin Intune.**

Navigați la Intune > **Utilizatori în** portalul Azure și verificați dacă utilizatorul nu este asociat la oricare dintre următoarele roluri în portalul Azure:

- Administrator global
- Administrator serviciu Intune
- Administrator SharePoint

Pentru mai multe informații, consultați [Controlul accesului bazat pe roluri (RBAC) cu Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Probleme de acces**

Pentru mai multe informații, consultați [Nu vă puteți conecta la Office 365, Azure sau Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).