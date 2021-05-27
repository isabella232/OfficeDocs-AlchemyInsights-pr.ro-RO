---
title: Depanarea redescoperirii ediscovery conține erori
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676280"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="3cb3c-102">Depanarea redescoperirii ediscovery conține erori</span><span class="sxs-lookup"><span data-stu-id="3cb3c-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="3cb3c-103">Aveți probleme în legătură cu descoperirea informațiilor electronic?</span><span class="sxs-lookup"><span data-stu-id="3cb3c-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="3cb3c-104">Iată câteva dintre cele mai bune practici de luat în considerare:</span><span class="sxs-lookup"><span data-stu-id="3cb3c-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="3cb3c-105">Verificați starea distribuției în așteptare.</span><span class="sxs-lookup"><span data-stu-id="3cb3c-105">Check the hold distribution status.</span></span>  <span data-ttu-id="3cb3c-106">Dacă starea este **On (În așteptare) sau** **Dezactivat (În așteptare),** așteptați să se finalizeze distribuirea.</span><span class="sxs-lookup"><span data-stu-id="3cb3c-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="3cb3c-107">Îmbinați actualizările pentru descoperirea informațiilor electronic într-o singură solicitare masivă, în loc să actualizați politica în mod repetat pentru fiecare tranzacție.</span><span class="sxs-lookup"><span data-stu-id="3cb3c-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="3cb3c-108">Rulați Set-CaseHoldPolicy <policyname> -RetryDistribution în Powershell Centrul de securitate și conformitate.</span><span class="sxs-lookup"><span data-stu-id="3cb3c-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="3cb3c-109">Pentru detalii, consultați [Consultați Conectare PowerShell pentru Centrul & securitate.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3cb3c-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="3cb3c-110">Pentru pașii necesari verificării acestor setări și a celor mai bune practici suplimentare pentru remedierea problemelor legate de descoperirea informațiilor electronic, consultați Depanarea erorilor de descoperire [a informațiilor electronic.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="3cb3c-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="3cb3c-111">Pentru informații despre depanarea altor probleme uzuale de descoperire a informațiilor electronic, consultați Investigarea, depanarea și [rezolvarea problemelor obișnuite de descoperire a informațiilor electronic.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="3cb3c-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
