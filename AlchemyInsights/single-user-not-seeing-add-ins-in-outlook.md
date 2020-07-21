---
title: Un singur utilizator nu vede programe de completare în Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198217"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="706a8-102">Un singur utilizator nu vede programe de completare în Outlook</span><span class="sxs-lookup"><span data-stu-id="706a8-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="706a8-103">Este posibil ca utilizatorul să facă parte dintr-un rol care nu are parametrul AppsForOfficeEnabled corect.</span><span class="sxs-lookup"><span data-stu-id="706a8-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="706a8-104">Executați acest cmdlet pentru a afla dacă rolul corect este asociat cu utilizatorul:</span><span class="sxs-lookup"><span data-stu-id="706a8-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="706a8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegarea $false | Format-Tabel -Rol automat,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="706a8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="706a8-106">Pentru mai multe informații, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="706a8-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
