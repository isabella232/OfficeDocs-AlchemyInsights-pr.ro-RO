---
title: Remedierea problemelor de livrare a mesajelor de e-mail în folderele publice activate pentru e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677940"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="193fd-102">Remedierea problemelor de livrare a mesajelor de e-mail în folderele publice activate pentru e-mail</span><span class="sxs-lookup"><span data-stu-id="193fd-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="193fd-103">Dacă expeditorii externi nu pot trimite mesaje în folderele publice activate pentru e-mail, iar expeditorii primesc eroarea: **nu s-a găsit (550 5.4.1)**, Verificați dacă domeniul de e-mail pentru folderul public este configurat ca domeniu de retransmisie internă în locul unui domeniu autoritar:</span><span class="sxs-lookup"><span data-stu-id="193fd-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="193fd-104">Deschideți [Centrul de administrare Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="193fd-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="193fd-105">Accesați domeniile acceptate pentru **flux de corespondență** \> **Accepted domains**, selectați domeniul acceptat, apoi faceți clic pe **Editare**.</span><span class="sxs-lookup"><span data-stu-id="193fd-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="193fd-106">În pagina proprietăți care se deschide, dacă tipul de domeniu este setat la **autoritate**, modificați valoarea la **retransmisie internă** , apoi faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="193fd-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="193fd-107">Dacă expeditorii externi primesc eroarea pe **care nu aveți permisiunea (550 5.7.13)**, derulează următoarea comandă în [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) pentru a vedea permisiunile pentru utilizatorii anonimi din folderul public:</span><span class="sxs-lookup"><span data-stu-id="193fd-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="193fd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` De exemplu, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="193fd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="193fd-109">Pentru a permite utilizatorilor externi să trimită mesaje de e-mail în acest folder public, adăugați direct CreateItems la utilizator Anonymous.</span><span class="sxs-lookup"><span data-stu-id="193fd-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="193fd-110">De exemplu, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="193fd-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
