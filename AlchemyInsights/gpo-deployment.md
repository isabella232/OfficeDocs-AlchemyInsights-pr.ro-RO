---
title: Implementare GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427562"
---
# <a name="gpo-deployment"></a>Implementare GPO

Setările pentru obiectele utilizator și computer din Azure Active Directory Domain Services (Azure AD DS) sunt deseori gestionate utilizând obiecte politică de grup (GPO). Azure AD DS include GPO-ul încorporat pentru AADDC utilizatori și containere pentru computere AADDC. Puteți să particularizați aceste GPO-ul încorporat pentru a configura politica de grup, după cum este necesar pentru mediul dvs. Membrii grupului Azure AD DC administratorii au privilegii de administrare a politicilor de grup în domeniul Azure AD DS și pot crea, de asemenea, GPO-ul particularizat și unitățile organizaționale (ou). Pentru mai multe informații despre politica de grup și cum funcționează, consultați [prezentarea generală a politicii de grup](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Într-un mediu hibrid, politicile de grup configurate într-un mediu AD DS local nu sunt sincronizate cu Azure AD DS. Pentru a defini setările de configurare pentru utilizatori sau computere în Azure AD DS, editați unul dintre GPO-ul implicit sau creați un GPO particularizat.

Acest articol [gestionarea politicii de grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vă arată cum să instalați instrumentele de gestionare a politicilor de grup, cum să editați tona în GPO-ul încorporat și cum să creați GPO particularizat.
