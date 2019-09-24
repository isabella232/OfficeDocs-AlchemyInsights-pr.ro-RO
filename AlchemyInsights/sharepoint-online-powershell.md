---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123010"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="e8c3a-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8c3a-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="e8c3a-103">Lucrul cu PowerShell sau scripturi în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e8c3a-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="e8c3a-104">Accesați linkurile de mai jos pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="e8c3a-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="e8c3a-105">Noțiuni introductive despre SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="e8c3a-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="e8c3a-106">Conectarea la SPO PowerShell cu autentificarea Multifactorial (MFA)</span><span class="sxs-lookup"><span data-stu-id="e8c3a-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="e8c3a-107">[Modele și practici SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) conține o bibliotecă de comenzi PowerShell care vă permite să efectuați acțiuni complexe de gestionare față de SPO.</span><span class="sxs-lookup"><span data-stu-id="e8c3a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="e8c3a-108">Dacă întâmpinați probleme la conectarea cu shell-ul de gestionare SPO, asigurați-vă că ați actualizat la cea mai recentă versiune și încercați să [importați din nou modulul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) utilizând *"import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="e8c3a-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="e8c3a-109">Dacă încercați să executați scripturi de model de obiect client-side, va trebui să aveți [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) instalat pe computerul local.</span><span class="sxs-lookup"><span data-stu-id="e8c3a-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="e8c3a-110">Dacă întâmpinați probleme la rularea script-uri din PowerShell, poate doriți să luați în considerare rularea PowerShell ca administrator și modificarea [politicii de executare](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="e8c3a-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>