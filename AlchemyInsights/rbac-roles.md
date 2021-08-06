---
title: 'Roluri RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923143"
---
# <a name="rbac-rules"></a>Reguli RBAC

Dacă obțineți eroarea de permisiune: 

- Clientul cu ID de obiect nu are autorizarea de a efectua o acțiune în domeniul de aplicare **(cod: AuthorizationFailed)**: atunci când încercați să creați o resursă, verificați dacă sunteți conectat în prezent cu un utilizator atribuit unui rol care are permisiune de scriere pentru resursă în domeniul selectat. De exemplu, pentru a gestiona mașini virtuale într-un grup de resurse, trebuie să aveți rolul [Colaborator](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) mașină virtuală în grupul de resurse (sau domeniul părinte). Pentru o listă de permisiuni pentru fiecare rol predefinit, consultați [Roluri predefinite pentru resurse Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Nu aveți permisiunea de **a** crea o solicitare de asistență: atunci când încercați să creați sau să actualizați un tichet de asistență, verificați dacă sunteți conectat în prezent cu un utilizator care are un rol care are permisiunea Microsoft.Support/supportTickets/write, cum ar fi Colaborator solicitare de [asistență.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Nu mai pot fi create atribuiri de roluri **(cod: RoleAssignmentLimitExceed)**: atunci când încercați să atribuiți un rol, încercați să reduceți numărul de atribuiri de roluri atribuind roluri unor grupuri. Azure acceptă până la **2000 de atribuiri** de roluri pentru fiecare abonament.

Pentru mai multe detalii despre rolurile Azure RBAC, [consultați Roluri Azure RBAC.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
