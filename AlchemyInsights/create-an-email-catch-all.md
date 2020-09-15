---
title: Crearea unui mesaj de e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712998"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b064a-102">Crearea unui mesaj de e-mail</span><span class="sxs-lookup"><span data-stu-id="b064a-102">Create an email catch all</span></span>

<span data-ttu-id="b064a-103">Utilizarea unei captură toate este puternic descurajată.</span><span class="sxs-lookup"><span data-stu-id="b064a-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b064a-104">Este mai bine să oferiți o revenire la expeditor, permițându-le expeditorilor să știe că mesajul său nu a putut fi livrat așa cum este adresat, astfel încât aceștia să poată lua măsuri.</span><span class="sxs-lookup"><span data-stu-id="b064a-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b064a-105">De asemenea, puteți limita cutia poștală monitorizată pentru a prinde doar adresele de e-mail valide anterior.</span><span class="sxs-lookup"><span data-stu-id="b064a-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b064a-106">Orice captură a cutiei poștale va primi o bună cantitate de spam și se poate umple în cele din urmă dacă nu este monitorizată îndeaproape.</span><span class="sxs-lookup"><span data-stu-id="b064a-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b064a-107">(Există limite de primire.)</span><span class="sxs-lookup"><span data-stu-id="b064a-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b064a-108">Dacă decideți să continuați, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="b064a-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b064a-109">Creați un grup de distribuire dinamic & includeți "toate tipurile de destinatari".</span><span class="sxs-lookup"><span data-stu-id="b064a-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b064a-110">Creați o cutie poștală dedicată pentru a prinde mesaje de e-mail, de exemplu, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="b064a-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b064a-111">Pentru domeniul specific, setați DomainType la "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="b064a-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b064a-112">Dacă mai târziu eliminați toate captură, asigurați-vă că setați domeniul înapoi la autoritate.</span><span class="sxs-lookup"><span data-stu-id="b064a-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b064a-113">Creați o regulă de transport fluxul după cum urmează:</span><span class="sxs-lookup"><span data-stu-id="b064a-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b064a-114">Dacă expeditorul este "în afara organizației"</span><span class="sxs-lookup"><span data-stu-id="b064a-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b064a-115">Redirecționați mesajul către Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="b064a-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b064a-116">Cu excepția cazului în care destinatarul este membru al allusers@domain.com (grupul de distribuire conține toți membrii)</span><span class="sxs-lookup"><span data-stu-id="b064a-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b064a-117">Asigurați-vă că validați noile cutii poștale sunt adăugate în grupul de distribuire dinamic</span><span class="sxs-lookup"><span data-stu-id="b064a-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
