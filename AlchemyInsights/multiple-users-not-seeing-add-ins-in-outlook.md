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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="75a38-102">Mai mulți utilizatori nu văd programe de completare în Outlook</span><span class="sxs-lookup"><span data-stu-id="75a38-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="75a38-103">Dacă testați programe de completare Outlook și niciunul nu apare, ca un prim pas de depanare, utilizați cmdlet-ul **Get-OrganizationConfig** PowerShell pentru a interoga parametrul _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="75a38-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="75a38-104">Dacă interogarea returnează o valoare **False**, setați acest parametru la **True** utilizând cmdlet-ul **Set-OrganizationConfig,** astfel încât programele de completare să apară conform așteptărilor.</span><span class="sxs-lookup"><span data-stu-id="75a38-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="75a38-105">Nu recomandăm ca parametrul _AppsForOfficeEnabled_ să fie setat la **False**.</span><span class="sxs-lookup"><span data-stu-id="75a38-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="75a38-106">O valoare a **False** suprascrie toate setările de rol administrative și de utilizator de mai sus și împiedică activarea oricăror aplicații noi de către orice utilizator din organizație.</span><span class="sxs-lookup"><span data-stu-id="75a38-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="75a38-107">Pentru mai multe informații, consultați [Specificarea administratorilor și utilizatorilor care pot instala și gestiona programe de completare pentru Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="75a38-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>