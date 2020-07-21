---
title: Ștergerea utilizatorului orfan de pe serverul local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198590"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="aba08-102">Ștergerea utilizatorului orfan de pe serverul local</span><span class="sxs-lookup"><span data-stu-id="aba08-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="aba08-103">Pentru a elimina un utilizator orfan, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="aba08-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="aba08-104">Forțați sincronizarea directorului urmând instrucțiunile din [Ce este identitatea hibridă cu Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="aba08-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="aba08-105">Pentru a verifica sincronizarea directorului, consultați [Ce este identitatea hibridă cu Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="aba08-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="aba08-106">Dacă sincronizarea funcționează corect, dar ștergerea obiectului Active Directory nu se propagă în Azure AD, eliminați manual obiectul orfan utilizând unul dintre următoarele module Azure Active Directory pentru cmdlet-urile Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="aba08-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="aba08-107">Eliminare-MsolContact</span><span class="sxs-lookup"><span data-stu-id="aba08-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="aba08-108">Eliminare-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="aba08-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="aba08-109">Eliminare-MsolUser</span><span class="sxs-lookup"><span data-stu-id="aba08-109">Remove-MsolUser</span></span>

    <span data-ttu-id="aba08-110">De exemplu, pentru a elimina ID-ul de utilizator orfan john.smith@contoso.com, creat inițial utilizând sincronizarea directorului, executați cmdlet::</span><span class="sxs-lookup"><span data-stu-id="aba08-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="aba08-111">Eliminare-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="aba08-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>