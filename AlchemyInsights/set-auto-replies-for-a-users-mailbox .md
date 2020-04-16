---
title: Setarea răspunsurilor automate pentru cutia poștală a unui utilizator
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506529"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="ec24f-102">Setarea răspunsurilor automate pentru cutia poștală a unui utilizator</span><span class="sxs-lookup"><span data-stu-id="ec24f-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="ec24f-103">**Metoda 1**</span><span class="sxs-lookup"><span data-stu-id="ec24f-103">**Method 1**</span></span>

1. <span data-ttu-id="ec24f-104">Conectați-vă la portalul Office 365</span><span class="sxs-lookup"><span data-stu-id="ec24f-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="ec24f-105">Accesați **Utilizatori > Utilizatori activi** (sau **Grupuri > Cutii poștale partajate** dacă ați setat într-o cutie poștală partajată).</span><span class="sxs-lookup"><span data-stu-id="ec24f-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="ec24f-106">Selectați un utilizator care are o cutie poștală Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec24f-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="ec24f-107">În meniul mobil din dreapta, accesați **Setări de e-mail > Răspunsuri automate** (dacă este vorba de o cutie poștală partajată, faceți pur și simplu clic pe **Răspunsuri automate** din meniul mobil).</span><span class="sxs-lookup"><span data-stu-id="ec24f-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="ec24f-108">**Metoda 2**</span><span class="sxs-lookup"><span data-stu-id="ec24f-108">**Method 2**</span></span>

1. <span data-ttu-id="ec24f-109">Conectați-vă la portalul de administrare Office 365 utilizând acreditări de administrator.</span><span class="sxs-lookup"><span data-stu-id="ec24f-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="ec24f-110">Extindeți **Centre de administrare**, apoi faceți clic pe **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ec24f-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="ec24f-111">Faceți clic pe imaginea din colțul din dreapta sus, pe **Alt utilizator**, apoi selectați cutia poștală de utilizator pe care doriți să o modificați.</span><span class="sxs-lookup"><span data-stu-id="ec24f-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="ec24f-112">În partea stângă, selectați **Opțiuni**, faceți clic pe **Organizare e-mail**, apoi pe **Răspunsuri automate.**</span><span class="sxs-lookup"><span data-stu-id="ec24f-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="ec24f-113">**Metoda 3**</span><span class="sxs-lookup"><span data-stu-id="ec24f-113">**Method 3**</span></span>

<span data-ttu-id="ec24f-114">Rulați următorul cmdlet în Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ec24f-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="ec24f-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="ec24f-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="ec24f-116">Pentru mai multe informații despre acest cmdlet, consultați [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="ec24f-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
