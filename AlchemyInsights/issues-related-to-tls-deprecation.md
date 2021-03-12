---
title: Nu se poate trimite/primi mesaje de e-mail la/de la Office 365 din cauza indisponibilității TLS 1,0 și TLS 1,1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747119"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="700e3-102">Nu se poate trimite/primi mesaje de e-mail la/de la Office 365 din cauza indisponibilității TLS 1,0 și TLS 1,1</span><span class="sxs-lookup"><span data-stu-id="700e3-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="700e3-103">Așa cum s-a confirmat de mesajul post Center MC229914, TLS 1,0 și TLS 1,1 au început impunerea pentru punctele finale pentru fluxul de corespondență Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="700e3-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="700e3-104">În curând Office 365 nu va mai accepta conexiuni de e-mail TLS 1,0 și TLS 1,1 din surse externe.</span><span class="sxs-lookup"><span data-stu-id="700e3-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="700e3-105">De asemenea, Exchange Online nu va utiliza niciodată TLS 1,0 sau 1,1 pentru a trimite mesaje de e-mail de ieșire.</span><span class="sxs-lookup"><span data-stu-id="700e3-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="700e3-106">Dacă întâmpinați probleme din cauza unei dezreușite TLS 1,0 sau 1,1, este posibil să vă confruntați cu una dintre următoarele erori-</span><span class="sxs-lookup"><span data-stu-id="700e3-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="700e3-107">Expeditorul devine NDR Bounce back-' 421 4.4.2 conexiune retrasă din cauza SocketError '</span><span class="sxs-lookup"><span data-stu-id="700e3-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="700e3-108">Eroare în vizualizatorul de cozi al serverului local, care trimite mesaje de e-mail către ofițer 365-' 421 conexiune 4.4.2 retrasă din cauza SocketError '</span><span class="sxs-lookup"><span data-stu-id="700e3-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="700e3-109">Eroare în Jurnalul de [protocoale](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) trimitere conector de pe serverul care trimite mesaje de E-mail la Office 365-TLS negociere nereușită cu eroarea SocketError</span><span class="sxs-lookup"><span data-stu-id="700e3-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="700e3-110">Eroare în Jurnalul de protocoale trimitere sau primire-' 451 5.7.3 trebuie să emită o comandă STARTTLS mai întâi '</span><span class="sxs-lookup"><span data-stu-id="700e3-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="700e3-111">Dacă întâmpinați oricare dintre erorile de mai sus, asigurați-vă că serverul care trimite sau primește mesaje de e-mail are TLS 1,2 activat, verificând următoarele chei de registry-</span><span class="sxs-lookup"><span data-stu-id="700e3-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="700e3-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="700e3-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="700e3-113">Dacă efectuați modificări în cheile de registry de mai sus pentru a activa TLS 1,2, reporniți serverul pentru ca modificările să aibă efect.</span><span class="sxs-lookup"><span data-stu-id="700e3-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="700e3-114">De asemenea, asigurați-vă că aveți instalate cele mai recente actualizări Windows și Exchange.</span><span class="sxs-lookup"><span data-stu-id="700e3-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="700e3-115">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="700e3-115">For more information, see:</span></span>

- [<span data-ttu-id="700e3-116">Orientare Exchange Server TLS, partea 1: pregătirea pentru TLS 1,2-comunitatea tehnică Microsoft</span><span class="sxs-lookup"><span data-stu-id="700e3-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="700e3-117">Partea de orientare Exchange Server TLS 2: Activarea TLS 1,2 și identificarea clienților care nu îl utilizează-comunitatea Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="700e3-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="700e3-118">Înțelegerea scenariilor de e-mail dacă versiunile TLS nu pot fi aprobate cu Exchange Online-comunitatea Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="700e3-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
