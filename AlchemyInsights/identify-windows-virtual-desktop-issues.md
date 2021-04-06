---
title: Identificarea problemelor cu desktopul virtual Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595857"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identificarea problemelor cu desktopul virtual Windows

Diagnosticarea desktop virtuală Windows utilizează un singur cmdlet PowerShell, dar conține mulți parametri opționali pentru a contribui la restrângerea și izolarea problemelor. Pentru a începe: 

1. Descărcați și importați modulul Windows Virtual Desktop PowerShell. Pentru detalii, consultați [Cmdleturi Desktop virtuale Windows pentru Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Rulați următorul cmdlet pentru a vă conecta la contul dvs.:
    
    Exemplu: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOTĂ:** Toate interogările care utilizează PowerShell trebuie să includă parametrii -UserName sau -ActivityID. Pentru capacități de monitorizare, consultați Utilizarea [analizelor jurnal pentru caracteristica de diagnosticare.](https://go.microsoft.com/fwlink/?linkid=2126847)

Pentru a filtra activitățile de diagnosticare după utilizator, rulați următorul cmdlet:

Exemplu: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Există o listă de filtre pe care le puteți rula pentru a diagnostica problemele. Pentru a afla mai multe despre diagnosticarea problemelor, consultați [Identificarea și diagnosticarea problemelor desktop virtuale Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Pentru a afla mai multe despre erorile comune, [consultați Erori comune senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
