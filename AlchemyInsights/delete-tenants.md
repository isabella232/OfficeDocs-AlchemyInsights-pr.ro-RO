---
title: Ștergerea entității găzduite
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564883"
---
# <a name="delete-tenant"></a>Ștergerea entității găzduite

Pentru a șterge o reclamă Azure, asigurați-vă:
- Sunteți administrator global în director.
- Nu sunteți conectat cu un cont care are directorul implicit, cum ar fi contoso.onmicrosoft.com, în contul conectat, cum ar fi admin@contoso.onmicrosoft.com.
- Eliminați toate aplicațiile active din Director înainte de ștergere. Pentru a elimina aplicațiile active, navigați la înregistrările aplicațiilor și eliminați aplicațiile existente.
- Nu există abonamente active pentru toate serviciile online Microsoft, cum ar fi Microsoft Azure, Office 365 sau Azure AD Premium asociate în director. Transferați abonamentele sau grăbiți anularea abonamentelor active prin suportul Azure și facturare. Aflați mai multe despre cum să anulați abonamentele Office 365 și Azure. Pentru instrucțiuni despre asocierea sau adăugarea unui abonament existent la o entitate găzduită, consultați [asocierea sau adăugarea unui abonament Azure la entitatea găzduită AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nu există nicio licență activă. Pentru a elimina licențele, consultați [cum să eliminați abonamentul pentru a elimina licența](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Nu există alți utilizatori activi în director, în afară de dvs., ca administrator global atunci când încercați să ștergeți reclama Azure. Eliminați orice alți utilizatori activi și toate dependențele unui nume de domeniu particularizat din entitatea găzduită vor trebui, de asemenea, eliminate, cum ar fi utilizatorii creați cu admin@contoso.com.

Pentru mai multe detalii despre cum să procedați:
- Ștergeți "Azure Active Directory" sau "abonament", consultați [ștergerea Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Eliminarea aplicațiilor din Director, consultați [eliminarea aplicațiilor](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
