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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067852"
---
# <a name="gpo-deployment"></a>Implementare GPO

Setări pentru obiecte de utilizator și computer din Azure Active Directory Domain Services (Azure AD DS) sunt gestionate adesea utilizând obiecte de politică de grup (GPOs). Azure AD DS include GPOs predefinit pentru containerele Utilizatori AADDC și Computere AADDC. Puteți particulariza aceste GPOs predefinite pentru a configura politica de grup după cum este necesar pentru mediul dvs. Membrii grupului de administratori Azure AD DC au privilegii de administrare a politicilor de grup în domeniul Azure AD DS și pot crea, de asemenea, GPOs particularizat și unități organizaționale (OUS). Pentru mai multe informații despre ce este politica de grup și cum funcționează aceasta, consultați Prezentare generală [a Politicii de grup.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Într-un mediu hibrid, politicile de grup configurate într-un mediu AD DS local nu sunt sincronizate cu Azure AD DS. Pentru a defini setările de configurare pentru utilizatori sau computere în Azure AD DS, editați unul dintre GPOs-urile implicite sau creați un GPO particularizat.

Acest articol [Gestionare politică](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) de grup vă arată cum să instalați instrumentele de gestionare a politicilor de grup, cum să editați tonă GPOs predefinit și cum să creați GPOs particularizat.
