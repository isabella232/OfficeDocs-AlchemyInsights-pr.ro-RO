---
title: Mai mulți utilizatori nu văd programe de completare în Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198239"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Mai mulți utilizatori nu văd programe de completare în Outlook

Dacă testați programe de completare Outlook și niciunul nu apare, ca un prim pas de depanare, utilizați cmdlet-ul **Get-OrganizationConfig** PowerShell pentru a interoga parametrul _AppsForOfficeEnabled._ Dacă interogarea returnează o valoare **False**, setați acest parametru la **True** utilizând cmdlet-ul **Set-OrganizationConfig,** astfel încât programele de completare să apară conform așteptărilor.

Nu recomandăm ca parametrul _AppsForOfficeEnabled_ să fie setat la **False**. O valoare a **False** suprascrie toate setările de rol administrative și de utilizator de mai sus și împiedică activarea oricăror aplicații noi de către orice utilizator din organizație.

Pentru mai multe informații, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).