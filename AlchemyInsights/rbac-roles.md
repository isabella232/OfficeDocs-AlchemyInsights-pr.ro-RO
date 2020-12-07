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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583950"
---
# <a name="rbac-rules"></a>Reguli RBAC

Dacă primiți eroarea de permisiune: 

- **Clientul cu ID obiect nu are autorizare pentru a efectua acțiuni peste domeniu (cod: AuthorizationFailed)**: atunci când încercați să creați o resursă, Verificați dacă sunteți conectat în prezent cu un utilizator căruia i se atribuie un rol care are permisiunea de scriere la resursă în domeniul selectat. De exemplu, pentru a gestiona mașini virtuale într-un grup de resurse, ar trebui să aveți rolul [contribuitor la mașina virtuală](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) în grupul resurse (sau în domeniul părinte). Pentru o listă a permisiunilor pentru fiecare rol predefinit, consultați [roluri predefinite pentru resurse Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Nu aveți permisiunea de a crea o solicitare de asistență**: atunci când încercați să creați sau să actualizați un tichet de asistență, Verificați dacă v-ați conectat în prezent cu un utilizator căruia i se atribuie un rol care are permisiunea Microsoft. Support/supportTickets/write, cum ar fi [contribuția la solicitarea de asistență](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nu se pot crea mai multe atribuiri de roluri (cod: RoleAssignmentLimitExceeded)**: când încercați să atribuiți un rol, încercați să reduceți numărul de atribuiri de roluri atribuind roluri în grupuri. Azure acceptă până la **2000** atribuiri de roluri pentru fiecare abonament.

Pentru mai multe detalii despre rolurile Azure RBAC, consultați [rolurile AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
