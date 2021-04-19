---
title: Exchange PowerShell și perimarea autentificării de bază
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813484"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="3a471-102">Exchange PowerShell și perimarea autentificării de bază</span><span class="sxs-lookup"><span data-stu-id="3a471-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="3a471-103">Pentru cele mai recente informații despre cum să vă conectați la Exchange Online PowerShell fără să utilizați autentificarea de bază, [accesați aici](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="3a471-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="3a471-104">Modulul PowerShell V2 nu utilizează autentificarea de bază.</span><span class="sxs-lookup"><span data-stu-id="3a471-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="3a471-105">Rețineți că autentificarea de bază trebuie să fie în continuare activată pe computerul client.</span><span class="sxs-lookup"><span data-stu-id="3a471-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="3a471-106">Noul modul PowerShell V2 utilizează Autentificarea modernă pentru a stabili o conexiune în vederea activării tuturor cmdleturilor V2 bazate pe REST.</span><span class="sxs-lookup"><span data-stu-id="3a471-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="3a471-107">Pe lângă cmdleturile V2, aveți permisiunea să accesați cmdleturile mai vechi PowerShell de la distanță (RPS) care necesită stabilirea unei sesiuni PowerShell la distanță.</span><span class="sxs-lookup"><span data-stu-id="3a471-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="3a471-108">Stabilirea unei sesiuni RPS pe computerul Windows necesită activarea WinRM BasicAuth pe computerul client, chiar dacă modulul utilizează mecanismul de Autentificare modernă pentru a se autentifica la serviciu.</span><span class="sxs-lookup"><span data-stu-id="3a471-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="3a471-109">Canalul WinRM Basic Auth este utilizat pentru transportul simbolurilor Autentificării moderne.</span><span class="sxs-lookup"><span data-stu-id="3a471-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="3a471-110">Dacă WinRM Basic Auth este dezactivată pe computerul client, noile cmdleturi V2 vor continua să funcționeze (dar cmdleturile RPS mai vechi nu vor mai funcționa).</span><span class="sxs-lookup"><span data-stu-id="3a471-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
