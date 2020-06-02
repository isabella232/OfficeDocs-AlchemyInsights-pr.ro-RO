---
title: Mutarea mesajelor de e-mail în cutia poștală Arhivă
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511052"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="f7d02-102">Mutarea e-mailului în cutia poștală de arhivă</span><span class="sxs-lookup"><span data-stu-id="f7d02-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="f7d02-103">Confirmați că a fost activată o **cutie poștală arhivă.**</span><span class="sxs-lookup"><span data-stu-id="f7d02-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="f7d02-104">Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) pentru a activa cutia poștală arhivă.</span><span class="sxs-lookup"><span data-stu-id="f7d02-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="f7d02-105">Pentru a arhiva automat mesajele în cutia poștală de arhivă, trebuie setată o etichetă de retenție cu acțiunea **Mutare în arhivă,** care trebuie setată automat **la întreaga etichetă poștală (implicită).**</span><span class="sxs-lookup"><span data-stu-id="f7d02-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="f7d02-106">Utilizați pașii de aici pentru a crea eticheta: [Eticheta implicită arhivă](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="f7d02-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="f7d02-107">Apoi, adăugați eticheta **Arhivă** la politica de conservare.</span><span class="sxs-lookup"><span data-stu-id="f7d02-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="f7d02-108">În centrul de administrare Exchange, alegeți **Politici de conservare** > **adăugați eticheta Mutare la arhivă** la politica > **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="f7d02-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="f7d02-109">Acum [atribuiți politica de conservare](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poștală a utilizatorului specific.</span><span class="sxs-lookup"><span data-stu-id="f7d02-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="f7d02-110">Aceeași politică se va aplica atât în **cutia poștală principală,** cât și în cutia poștală **arhivă.**</span><span class="sxs-lookup"><span data-stu-id="f7d02-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="f7d02-111">Poate fi necesar să forțați Asistentul de foldere gestionate (AMF) să execute și să aplice noile setări cutiei poștale a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="f7d02-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="f7d02-112">Executați următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni Asistent folder gestionat pentru o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="f7d02-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="f7d02-113">Identitate a unui folder gestionat de pornire<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="f7d02-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="f7d02-114">Pentru mai multe informații despre configurarea unei politici de arhivare, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="f7d02-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  