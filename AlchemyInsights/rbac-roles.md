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
# <a name="rbac-rules"></a><span data-ttu-id="8474c-102">Reguli RBAC</span><span class="sxs-lookup"><span data-stu-id="8474c-102">RBAC rules</span></span>

<span data-ttu-id="8474c-103">Dacă primiți eroarea de permisiune:</span><span class="sxs-lookup"><span data-stu-id="8474c-103">If you get the permission error:</span></span> 

- <span data-ttu-id="8474c-104">**Clientul cu ID obiect nu are autorizare pentru a efectua acțiuni peste domeniu (cod: AuthorizationFailed)**: atunci când încercați să creați o resursă, Verificați dacă sunteți conectat în prezent cu un utilizator căruia i se atribuie un rol care are permisiunea de scriere la resursă în domeniul selectat.</span><span class="sxs-lookup"><span data-stu-id="8474c-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="8474c-105">De exemplu, pentru a gestiona mașini virtuale într-un grup de resurse, ar trebui să aveți rolul [contribuitor la mașina virtuală](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) în grupul resurse (sau în domeniul părinte).</span><span class="sxs-lookup"><span data-stu-id="8474c-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="8474c-106">Pentru o listă a permisiunilor pentru fiecare rol predefinit, consultați [roluri predefinite pentru resurse Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8474c-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="8474c-107">**Nu aveți permisiunea de a crea o solicitare de asistență**: atunci când încercați să creați sau să actualizați un tichet de asistență, Verificați dacă v-ați conectat în prezent cu un utilizator căruia i se atribuie un rol care are permisiunea Microsoft. Support/supportTickets/write, cum ar fi [contribuția la solicitarea de asistență](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="8474c-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="8474c-108">**Nu se pot crea mai multe atribuiri de roluri (cod: RoleAssignmentLimitExceeded)**: când încercați să atribuiți un rol, încercați să reduceți numărul de atribuiri de roluri atribuind roluri în grupuri.</span><span class="sxs-lookup"><span data-stu-id="8474c-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="8474c-109">Azure acceptă până la **2000** atribuiri de roluri pentru fiecare abonament.</span><span class="sxs-lookup"><span data-stu-id="8474c-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="8474c-110">Pentru mai multe detalii despre rolurile Azure RBAC, consultați [rolurile AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8474c-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
