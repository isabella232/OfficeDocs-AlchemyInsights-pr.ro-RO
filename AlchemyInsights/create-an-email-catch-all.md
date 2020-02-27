---
title: Creați o captură prin e-mail pe toate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286204"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="0535d-102">Creați o captură prin e-mail pe toate</span><span class="sxs-lookup"><span data-stu-id="0535d-102">Create an email catch all</span></span>

<span data-ttu-id="0535d-103">Utilizarea unei capturi toate este puternic descurajat.</span><span class="sxs-lookup"><span data-stu-id="0535d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="0535d-104">Este mai bine pentru a oferi o saritura înapoi la expeditor închirierea expeditorilor știu mesajul lor nu a putut fi livrate ca abordate, astfel încât acestea să poată lua măsuri.</span><span class="sxs-lookup"><span data-stu-id="0535d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="0535d-105">De asemenea, puteți limita cutia poștală monitorizată pentru a prinde numai adresele de e-mail valide anterior.</span><span class="sxs-lookup"><span data-stu-id="0535d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="0535d-106">Orice captură toate cutia poștală va primi o afacere bună de spam și poate umple în cele din urmă, dacă nu monitorizate îndeaproape.</span><span class="sxs-lookup"><span data-stu-id="0535d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="0535d-107">(Există limite de primire.)</span><span class="sxs-lookup"><span data-stu-id="0535d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="0535d-108">Dacă decideți să continuați, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="0535d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="0535d-109">Creați un grup de distribuire dinamic & include "Toate tipurile de destinatari".</span><span class="sxs-lookup"><span data-stu-id="0535d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="0535d-110">Creați o cutie poștală dedicată pentru a prinde e-mailuri, de exemplu, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="0535d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="0535d-111">Pentru domeniul specific, setați DomainType la "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="0535d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="0535d-112">Dacă mai târziu eliminați captura toate, asigurați-vă că pentru a seta domeniul înapoi la cu autoritate.</span><span class="sxs-lookup"><span data-stu-id="0535d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="0535d-113">Creați o regulă de transport mailflow după urmează:</span><span class="sxs-lookup"><span data-stu-id="0535d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="0535d-114">Dacă Expeditorul este "În afara organizației"</span><span class="sxs-lookup"><span data-stu-id="0535d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="0535d-115">Redirecționați mesajul către Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="0535d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="0535d-116">Cu excepția cazului în care destinatarul este membru al allusers@domain.com (Grupul de distribuire conține toți membrii)</span><span class="sxs-lookup"><span data-stu-id="0535d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="0535d-117">Asigurați-vă că pentru a valida că noile cutii poștale sunt adăugate în grupul de distribuire dinamică</span><span class="sxs-lookup"><span data-stu-id="0535d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
