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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522783"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="72ef3-102">Mutarea e-mailului în cutia poștală de arhivă</span><span class="sxs-lookup"><span data-stu-id="72ef3-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="72ef3-103">Dacă doriți să executăm verificări automate pentru setările menționate mai jos, selectați butonul din spate <-- în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme în mutarea e-mailului în cutia poștală de arhivă.</span><span class="sxs-lookup"><span data-stu-id="72ef3-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="72ef3-104">Confirmați că a fost activată o **cutie poștală Arhivă.**</span><span class="sxs-lookup"><span data-stu-id="72ef3-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="72ef3-105">Dacă nu, utilizați pașii din [acest articol](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) pentru a activa cutia poștală de arhivă.</span><span class="sxs-lookup"><span data-stu-id="72ef3-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="72ef3-106">Pentru a arhiva automat mesajele în cutia poștală de arhivă, o etichetă de retenție cu acțiunea **Mutare în arhivă** trebuie setată automat la eticheta **aplicată automat întregii cutii poștale (implicit).**</span><span class="sxs-lookup"><span data-stu-id="72ef3-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="72ef3-107">Utilizați pașii de aici pentru a crea eticheta: [Arhivați eticheta implicită](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="72ef3-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="72ef3-108">Apoi, adăugați eticheta **Arhivă** la politica de retenție.</span><span class="sxs-lookup"><span data-stu-id="72ef3-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="72ef3-109">În centrul de administrare Exchange, alegeți **Politici de retenție** > **adăugați eticheta Mutare la arhivă** la politica > **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="72ef3-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="72ef3-110">Acum [atribuiți politica de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cutiei poștale a utilizatorului respectiv.</span><span class="sxs-lookup"><span data-stu-id="72ef3-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="72ef3-111">Aceeași politică se va aplica atât cutiei **poștale Primară,** cât și cutiei poștale **Arhivă.**</span><span class="sxs-lookup"><span data-stu-id="72ef3-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="72ef3-112">Poate fi necesar să forțați Asistentul de foldere gestionate (MFA) să ruleze și să aplice noile setări cutiei poștale a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="72ef3-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="72ef3-113">Executați următoarea comandă în timp ce [sunteți conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni Asistentul de foldere gestionate pentru o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="72ef3-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="72ef3-114">Pornire-gestionatFolderAssistant -Identitate<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="72ef3-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="72ef3-115">Pentru mai multe informații despre configurarea unei politici de arhivă, consultați [Configurarea unei politici de arhivare și ștergere pentru cutiile poștale](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="72ef3-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  