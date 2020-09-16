---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770851"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6c893-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="6c893-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6c893-103">Lucrați cu PowerShell sau cu scripturi în SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6c893-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6c893-104">Accesați linkurile de mai jos pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="6c893-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6c893-105">Introducere în componenta de administrare SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6c893-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6c893-106">Conectarea la SPO PowerShell cu autentificarea prin multifactor (AMF)</span><span class="sxs-lookup"><span data-stu-id="6c893-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6c893-107">[Modele și practici SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) conține o bibliotecă de comenzi PowerShell care vă permite să efectuați acțiuni complexe de gestionare către SPO.</span><span class="sxs-lookup"><span data-stu-id="6c893-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6c893-108">Dacă întâmpinați probleme la conectarea cu componenta de administrare SPO, asigurați-vă că ați actualizat la cea mai recentă versiune și încercați să [reimportați modulul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) utilizând *"import-modulul Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6c893-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6c893-109">Dacă încercați să setați Scripturile model de obiecte de pe partea client, va trebui să aveți instalat [SDK-ul componente client SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) pe computerul local.</span><span class="sxs-lookup"><span data-stu-id="6c893-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6c893-110">Dacă întâmpinați probleme la executarea scripturilor din PowerShell, poate că doriți să luați în considerare executarea PowerShell ca administrator și modificarea [politicii de execuție](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6c893-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>