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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Un singur utilizator nu vede programe de completare în Outlook

Este posibil ca utilizatorul să facă parte dintr-un rol care nu are parametrul AppsForOfficeEnabled corect. Executați acest cmdlet pentru a afla dacă rolul corect este asociat cu utilizatorul:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegarea $false | Format-Tabel -Rol automat,RoleAssigneeName,RoleAssigneeType

Pentru mai multe informații, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
