---
title: Mai mulți utilizatori primesc eroare Access Denied în timp ce adaugă programe de completare în Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424172"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="18065-102">Mai mulți utilizatori primesc eroare Access Denied în timp ce adaugă programe de completare în Outlook</span><span class="sxs-lookup"><span data-stu-id="18065-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="18065-103">Aveți posibilitatea să specificați administratorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="18065-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="18065-104">De asemenea, aveți posibilitatea să specificați ce utilizatori din organizație au permisiunea de a instala și gestiona programele de completare pentru uz propriu.</span><span class="sxs-lookup"><span data-stu-id="18065-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="18065-105">Pentru detalii, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="18065-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="18065-106">Pentru a verifica dacă ați atribuit cu succes permisiuni pentru un utilizator, înlocuiți <Role Name> cu numele rolului de verificat și executați următoarea comandă în Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="18065-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="18065-107">Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="18065-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="18065-108">Acest exemplu vă arată să verificați cui le-ați atribuit permisiuni pentru a instala programe de completare din Magazinul Office pentru organizație.</span><span class="sxs-lookup"><span data-stu-id="18065-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="18065-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="18065-109">PowerShell</span></span>

<span data-ttu-id="18065-110">-Rolul "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="18065-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="18065-111">În rezultate, Get-ManagementRoleAssignment, revizuiți intrările din coloana Utilizatori eficienți.</span><span class="sxs-lookup"><span data-stu-id="18065-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="18065-112">Pentru informații detaliate despre sintaxă și parametri, consultați [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="18065-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 