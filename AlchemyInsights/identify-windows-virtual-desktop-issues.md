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
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="08273-102">Identificarea problemelor cu desktopul virtual Windows</span><span class="sxs-lookup"><span data-stu-id="08273-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="08273-103">Diagnosticarea desktop virtuală Windows utilizează un singur cmdlet PowerShell, dar conține mulți parametri opționali pentru a contribui la restrângerea și izolarea problemelor.</span><span class="sxs-lookup"><span data-stu-id="08273-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="08273-104">Pentru a începe:</span><span class="sxs-lookup"><span data-stu-id="08273-104">To get started:</span></span> 

1. <span data-ttu-id="08273-105">Descărcați și importați modulul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="08273-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="08273-106">Pentru detalii, consultați [Cmdleturi Desktop virtuale Windows pentru Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="08273-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="08273-107">Rulați următorul cmdlet pentru a vă conecta la contul dvs.:</span><span class="sxs-lookup"><span data-stu-id="08273-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="08273-108">Exemplu: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="08273-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="08273-109">**NOTĂ:** Toate interogările care utilizează PowerShell trebuie să includă parametrii -UserName sau -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="08273-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="08273-110">Pentru capacități de monitorizare, consultați Utilizarea [analizelor jurnal pentru caracteristica de diagnosticare.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="08273-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="08273-111">Pentru a filtra activitățile de diagnosticare după utilizator, rulați următorul cmdlet:</span><span class="sxs-lookup"><span data-stu-id="08273-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="08273-112">Exemplu: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="08273-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="08273-113">Există o listă de filtre pe care le puteți rula pentru a diagnostica problemele.</span><span class="sxs-lookup"><span data-stu-id="08273-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="08273-114">Pentru a afla mai multe despre diagnosticarea problemelor, consultați [Identificarea și diagnosticarea problemelor desktop virtuale Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="08273-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="08273-115">Pentru a afla mai multe despre erorile comune, [consultați Erori comune senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="08273-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
