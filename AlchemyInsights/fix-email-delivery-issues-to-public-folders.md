---
title: Remedierea problemelor de livrare a e-mailurilor în folderele publice activate pentru e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716364"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="17d24-102">Remedierea problemelor de livrare a e-mailurilor în folderele publice activate pentru e-mail</span><span class="sxs-lookup"><span data-stu-id="17d24-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="17d24-103">Dacă expeditorii externi nu pot trimite mesaje către folderele publice activate pentru e-mail, iar expeditorii primesc eroarea: **nu s-a găsit (550 5.4.1),** verificați că domeniul de poștă electronică pentru folderul public este configurat ca domeniu intern de retransmisie în locul unui domeniu cu autoritate:</span><span class="sxs-lookup"><span data-stu-id="17d24-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="17d24-104">Deschideți centrul de [administrare Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="17d24-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="17d24-105">Accesați **Flux de** \> **corespondență Domenii acceptate**, selectați domeniul acceptat, apoi faceți clic pe **Editare**.</span><span class="sxs-lookup"><span data-stu-id="17d24-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="17d24-106">În pagina de proprietăți care se deschide, dacă tipul de domeniu este setat la **Autoritate**, modificați valoarea la **Releu intern,** apoi faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="17d24-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="17d24-107">Dacă expeditorii externi primesc eroarea **nu aveți permisiunea (550 5.7.13),** executați următoarea comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi în folderul public:</span><span class="sxs-lookup"><span data-stu-id="17d24-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="17d24-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="17d24-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="17d24-109">Pentru a permite utilizatorilor externi să trimită e-mailuri în acest folder public, adăugați dreptul de acces CreateItems la utilizatorul Anonim.</span><span class="sxs-lookup"><span data-stu-id="17d24-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="17d24-110">De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="17d24-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
