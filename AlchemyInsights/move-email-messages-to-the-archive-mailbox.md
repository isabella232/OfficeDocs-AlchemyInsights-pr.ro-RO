---
title: Mutarea mesajelor de poștă electronică în cutia poștală arhivă
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822174"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="f08a6-102">Mutarea e-mailului în cutia poștală arhivă</span><span class="sxs-lookup"><span data-stu-id="f08a6-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="f08a6-103">Confirmați că a fost activată o **cutie poștală arhivă** .</span><span class="sxs-lookup"><span data-stu-id="f08a6-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="f08a6-104">Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pentru a activa cutia poștală de arhivă.</span><span class="sxs-lookup"><span data-stu-id="f08a6-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="f08a6-105">Pentru a arhiva mesajele automat la cutia poștală de arhivă, o etichetă de retenție cu **Mutare în arhivă** acțiune trebuie setată la **aplicată automat la întreaga cutie poștală (implicit) etichetă**.</span><span class="sxs-lookup"><span data-stu-id="f08a6-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="f08a6-106">Utilizați pașii de aici pentru a crea eticheta: [arhivați eticheta implicită](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="f08a6-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="f08a6-107">Apoi, adăugați eticheta de **arhivă** la Politica de retenție.</span><span class="sxs-lookup"><span data-stu-id="f08a6-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="f08a6-108">În centrul de administrare Exchange, alegeți **politicile de conservare** > adăugați **mutați în arhiva etichetă** la politica > **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="f08a6-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="f08a6-109">Acum [atribuiți Politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poștală a utilizatorului specific.</span><span class="sxs-lookup"><span data-stu-id="f08a6-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="f08a6-110">Aceeași politică se va aplica atât la cutia poștală **principală** și **arhivă** .</span><span class="sxs-lookup"><span data-stu-id="f08a6-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="f08a6-111">Poate fi necesar să forțați asistentul pentru foldere gestionate (MFA) să ruleze și să aplice noile setări la cutia poștală a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="f08a6-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="f08a6-112">Executați următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul de foldere gestionate pentru o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="f08a6-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="f08a6-113">Start-ManagedFolderAssistant-identitate<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="f08a6-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="f08a6-114">Pentru mai multe informații despre configurarea unei politici de arhivă, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="f08a6-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  