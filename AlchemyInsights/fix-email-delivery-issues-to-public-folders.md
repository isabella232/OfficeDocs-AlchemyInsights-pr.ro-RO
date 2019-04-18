---
title: Rezolva problemele de livrare e-mail la folderele publice cu corespondenţa activată
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910621"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="5f578-102">Rezolva problemele de livrare e-mail la folderele publice cu corespondenţa activată</span><span class="sxs-lookup"><span data-stu-id="5f578-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="5f578-103">Dacă expeditori externi nu pot trimite mesaje la folderele publice cu corespondenţa activată şi expeditorii primesc eroare: **nu a putut fi găsit (550 5.4.1)**, verificaţi dacă domeniul de e-mail pentru folderul public este configurat ca domeniu intern de retransmisie în loc de o domeniu de autoritate:</span><span class="sxs-lookup"><span data-stu-id="5f578-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="5f578-104">Deschideţi [Centrul de administrare Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="5f578-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="5f578-105">Du-te la **fluxul de corespondenţă** \> **acceptat domenii**, selectaţi domeniul acceptat, şi apoi faceţi clic pe **Editare**.</span><span class="sxs-lookup"><span data-stu-id="5f578-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="5f578-106">În proprietăţile paginii care se deschide, în cazul în care tipul de domeniu este setată la **Authoritative**, value la spre **intern de retransmisie** şi apoi faceţi clic pe **salvaţi**.</span><span class="sxs-lookup"><span data-stu-id="5f578-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="5f578-107">Dacă expeditori externi primesc eroare, **nu aveţi permisiunea (550 5.7.13)**, executaţi comanda următoare în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi în folderul public:</span><span class="sxs-lookup"><span data-stu-id="5f578-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="5f578-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="5f578-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="5f578-109">Pentru a permite utilizatorilor externi să trimite email pentru acest folder public, Adauga acces CreateItems dreptul la utilizator anonim.</span><span class="sxs-lookup"><span data-stu-id="5f578-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="5f578-110">De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="5f578-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
