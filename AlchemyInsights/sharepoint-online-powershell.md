---
title: Sharepoint Online PowerShell
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
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830594"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="50aa0-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="50aa0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="50aa0-103">Lucrați cu PowerShell sau scripturi în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="50aa0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="50aa0-104">Vizitați linkurile de mai jos pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="50aa0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="50aa0-105">Noțiuni de bază pentru Partea de administrare SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="50aa0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="50aa0-106">Conectarea la SPO PowerShell cu multi-factor authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="50aa0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="50aa0-107">[Modelele și practicile SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) conțin o bibliotecă de comenzi PowerShell care vă permite să efectuați acțiuni complexe de gestionare către SPO.</span><span class="sxs-lookup"><span data-stu-id="50aa0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="50aa0-108">Dacă aveți probleme la conectarea cu shell-ul de gestionare SPO, [asigurați-vă](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) că ați actualizat la cea mai recentă versiune și încercați să importați din nou modulul utilizând *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="50aa0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="50aa0-109">Dacă încercați să rulați scripturi de model de obiecte pe partea client, va trebui să aveți SDK Componente [client Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) instalat pe computerul local.</span><span class="sxs-lookup"><span data-stu-id="50aa0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="50aa0-110">Dacă aveți probleme cu rularea scripturilor din PowerShell, se recomandăm să luați în considerare rularea PowerShell ca Administrator și să modificați Politica [de executare.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="50aa0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>