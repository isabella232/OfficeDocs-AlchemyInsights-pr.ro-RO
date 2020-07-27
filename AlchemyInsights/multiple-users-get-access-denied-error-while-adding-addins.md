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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Mai mulți utilizatori primesc eroare Access Denied în timp ce adaugă programe de completare în Outlook

Aveți posibilitatea să specificați administratorii din organizația dvs. De asemenea, aveți posibilitatea să specificați ce utilizatori din organizație au permisiunea de a instala și gestiona programele de completare pentru uz propriu.

Pentru detalii, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Pentru a verifica dacă ați atribuit cu succes permisiuni pentru un utilizator, înlocuiți <Role Name> cu numele rolului de verificat și executați următoarea comandă în Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

Acest exemplu vă arată să verificați cui le-ați atribuit permisiuni pentru a instala programe de completare din Magazinul Office pentru organizație.

Powershell

-Rolul "Org Marketplace Apps" -GetEffectiveUsers

În rezultate, Get-ManagementRoleAssignment, revizuiți intrările din coloana Utilizatori eficienți.

Pentru informații detaliate despre sintaxă și parametri, consultați [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 