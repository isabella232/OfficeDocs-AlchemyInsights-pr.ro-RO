---
title: Utilizați Windows PowerShell pentru partajarea politicilor și a relațiilor dintre organizații
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998479"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Utilizați Windows PowerShell pentru partajarea politicilor și a relațiilor dintre organizații


Pentru relațiile dintre organizații, revizuiți sintaxa detaliată și informațiile despre parametri pentru: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ȘI  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Pentru a crea o politică de partajare, utilizați[New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Pentru  [a aplica o politică de partajare la o cutie poștală sau la un utilizator](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes),  trebuie să utilizați o combinație de  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) și [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) cu politica nou creată. Pentru  [a modifica, a dezactiva sau a elimina o politică de partajare](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy),  trebuie să utilizați  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) și [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pentru a înțelege complet acest subiect, citiți:**

[Partajarea în Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)