---
title: Testarea configurației IRM pentru noi capacități OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812444"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testarea configurației IRM pentru noi capacități OME

Pentru a verifica dacă entitatea Microsoft 365 găzduită este configurată să utilizeze noi capacități OME, rulați următoarele cmdleturi în timp ce sunteți [conectat la Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Verificați configurația IRM a entității găzduite rulezând `Get-IRMConfiguration` . Asigurați-vă că aceste valori sunt setate **la True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Utilizând domeniul, adresa expeditorului și destinatarul, rulați `Test-IRMConfiguration` . Dacă testul nu trece, investigați configurația IRM.

Pentru mai multe informații despre verificarea configurației IRM, consultați [Verificarea noii configurații OME în Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)