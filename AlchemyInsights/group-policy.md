---
title: Politica de grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256785"
---
# <a name="group-policy"></a>Politica de grup

Setările pentru obiectele utilizator și computer din Azure Active Directory Domain Services (Azure AD DS) sunt deseori gestionate utilizând obiecte politică de grup (GPO). Azure AD DS include GPO-ul încorporat pentru AADDC utilizatori și containere pentru computere AADDC. Puteți să particularizați aceste GPO-ul încorporat pentru a configura politica de grup, după cum este necesar pentru mediul dvs. Membrii grupului Azure AD DC administratorii au privilegii de administrare a politicilor de grup în domeniul Azure AD DS și pot crea, de asemenea, GPO-ul particularizat și unitățile organizaționale (ou). Pentru mai multe informații despre politica de grup și cum funcționează, consultați [prezentarea generală a politicii de grup](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Într-un mediu hibrid, politicile de grup configurate într-un mediu AD DS local nu sunt sincronizate cu Azure AD DS. Pentru a defini setările de configurare pentru utilizatori sau computere în Azure AD DS, editați unul dintre GPO-ul implicit sau creați un GPO particularizat.

Acest articol [gestionarea politicii de grup](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vă arată cum să instalați instrumentele de gestionare a politicilor de grup, cum să editați tona în GPO-ul încorporat și cum să creați GPO particularizat.



