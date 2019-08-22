---
title: Eroare trimitere e-mail blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527153"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="98ccc-102">Eroare trimitere e-mail: clientul gazdă blocat folosind Spamhaus</span><span class="sxs-lookup"><span data-stu-id="98ccc-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="98ccc-103">IP-ul care a trimis mesajul este pe o listă de bloc, deţinut de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="98ccc-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="98ccc-104">Motivele fiind blocate de Spamhaus includ conturi compromise, compromisă masini schimb o adresă IP publică și politici de furnizorul de servicii Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="98ccc-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="98ccc-105">Remedierile posibile sunt:</span><span class="sxs-lookup"><span data-stu-id="98ccc-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="98ccc-106">Pentru mesajele de intrare blocat la Office 365 în cazul în care aveţi de a controla sursa de server de e-mail, aveţi nevoie pentru a determina cauza şi de a elimina bloc din site-ul Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="98ccc-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="98ccc-107">Blocat mesaje de intrare la Office 365 în cazul în care adresa de IP a sursei aparţine altcuiva, adresa proprietarului trebuie să scoateţi blocul Spamhaus pe site-ul.</span><span class="sxs-lookup"><span data-stu-id="98ccc-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="98ccc-108">Dacă adresa IP este pe lista de bloc Politica (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa de PBL.</span><span class="sxs-lookup"><span data-stu-id="98ccc-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="98ccc-109">Pentru mesajele de ieşire blocate din domeniul Office 365, puteţi primi această eroare în cazul în care mesajele sunt dirijate printr-un serviciu de 3rd party.</span><span class="sxs-lookup"><span data-stu-id="98ccc-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="98ccc-110">Utilizaţi un instrument de căutare WHOIS pentru a găsi proprietarul de adrese IP blocate.</span><span class="sxs-lookup"><span data-stu-id="98ccc-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
