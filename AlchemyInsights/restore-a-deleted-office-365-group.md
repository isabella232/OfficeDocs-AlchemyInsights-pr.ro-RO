---
title: Restaurarea unui grup Microsoft 365 șters
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645143"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="34242-102">Restaurarea unui grup Microsoft 365 șters</span><span class="sxs-lookup"><span data-stu-id="34242-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="34242-103">Puteți restaura un grup Microsoft 365 șters sau Microsoft Teams în termen de 30 de zile de la ștergere.</span><span class="sxs-lookup"><span data-stu-id="34242-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="34242-104">Accesați Centrul de [administrare Microsoft 365](https://aka.ms/RestoreDeletedGroup) pentru a vă conecta la o listă cu grupurile și echipele șterse.</span><span class="sxs-lookup"><span data-stu-id="34242-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="34242-105">**Notă:** Conectați-vă utilizând contul care este atribuit administratorului entității găzduite sau rolului de administrator al grupurilor.</span><span class="sxs-lookup"><span data-stu-id="34242-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="34242-106">Selectați grupul Microsoft 365 șters/Teams pentru a fi restaurat și dați clic pe **Restabiliți grupul**.</span><span class="sxs-lookup"><span data-stu-id="34242-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="34242-107">Dacă grupul nu poate fi restaurat din cauza unei adrese SMTP conflictuale, utilizați următoarea comandă pentru a găsi obiectul care provoacă conflictul și eliminați adresa SMTP:</span><span class="sxs-lookup"><span data-stu-id="34242-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="34242-108">**Notă:** În unele cazuri, poate dura 24 de ore pentru ca grupul și toate datele sale să fie restaurate.</span><span class="sxs-lookup"><span data-stu-id="34242-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="34242-109">Pentru mai multe informații sau pentru a afla cum să restaurați grupuri utilizând PowerShell, consultați [Restaurarea unui grup Microsoft 365 șters.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="34242-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>