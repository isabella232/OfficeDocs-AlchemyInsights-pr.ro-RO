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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993905"
---
# <a name="delete-tenant"></a>Ștergerea entității găzduite

Pentru a șterge un Azure AD, asigurați-vă că:
- Sunteți administrator global în director.
- NU sunteți conectat cu un cont care are directorul implicit, cum ar fi contul contoso.onmicrosoft.com conectat, cum ar fi un cont de admin@contoso.onmicrosoft.com.
- Eliminați toate aplicațiile active din director înainte de ștergere. Pentru a elimina aplicațiile active, navigați la înregistrările de aplicații și eliminați aplicațiile existente.
- Nu există abonamente active pentru niciun serviciu Microsoft Online Services, cum ar fi servicii Microsoft Azure, Office 365 sau Azure AD Premium în director. Transferați abonamentele sau anularea accelerată a abonamentelor active prin asistența și facturarea Azure. Aflați mai multe despre Anularea abonamentelor Office 365 Azure. Pentru instrucțiuni despre asocierea sau adăugarea unui abonament existent la o entitate găzduită, consultați Asocierea sau adăugarea unui abonament Azure la entitatea [găzduită Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nu există nicio licență activă. Pentru a elimina licențe, consultați [Cum se elimină abonamentul pentru a elimina licența](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Nu mai există alți utilizatori activi în director în afară de dvs., ca administrator global, atunci când încercați să ștergeți Azure AD. Eliminați toți ceilalți utilizatori activi și orice dependențe de un nume de domeniu particularizat din entitatea găzduită vor trebui, de asemenea, eliminate, cum ar fi utilizatorii creați cu admin@contoso.com.

Pentru mai multe detalii despre:
- Ștergeți "Azure Active Directory" sau "abonament", consultați [Ștergerea Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Eliminarea aplicațiilor din director, consultați [Eliminarea aplicațiilor.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
